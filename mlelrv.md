代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgekhdfj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cjvhghsu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mirxzhtn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hselkmmu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3igrftjnp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vwqeyven.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mbmphljf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lkfndduw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osgpwjmd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hexrqtjd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bnavwrkk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3btkqdgkf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3utwwpccy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vstncrrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lijrnebi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xoiwqujj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vawgydrm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gzaaunnr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tcecvbhw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tqwauxjz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vgtgbpnc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mgampqhq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wyvltwmp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3eoufzpmy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qwqnlbrs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hnwzfwuv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3llvmygvz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3aowauilp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tvfrztdn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ficxbwve.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cfzcsore.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ldmvuezx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nfosqqds.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uodnnskx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ldcwqfxx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wgazrcwi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uawukztp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vdaavari.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wjzbzunh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pdkeubhx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gcsqpinh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ltgoqjkn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3egldjfhg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uvwrlyox.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kccubsqu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3afoehtse.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dcecdikj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jldsaufa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cfpjqzgr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ygumabbg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cmeayxcq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bfvrjpkt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvfisggb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ycnioyla.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kwptoksk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ygrevkfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gllqqvvz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfkrodgj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3igaedjnw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lpkfsrpo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kxpqnval.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kfljbjhm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dyigtdhs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3flwlmnvx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3otrogogl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usgoalrb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3inandfkt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gyncwhjb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3achrczbq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3datbtqdh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3sfmhzcra.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xtictzdd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jhtwrakl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jybiblfm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gcqvways.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbmztjhg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3oobobsdg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3osgjhtkh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxyhsquu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrivlvyf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kunbjlhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhpyaeji.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sxjapgkr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3llbvbvpy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kknnxpbg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ciqgknlm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3znfsbkvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ijqvuduc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jcnflfoh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jdbxzfrf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qwjbjzof.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3udiglbcm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hwretcgk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vpozgacf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3biymkmaa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gjokvkwl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eppyddmu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdhhtxy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tekeyulb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ralosibq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bkckzxsl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qrsonhgt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ynhowqxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3advyaeek.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3psnrqvrw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ehfjxspl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jkduoyqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fkozeabl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xysjxusj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lekvyhyz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nxbasphn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wxoztoox.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3emlthheg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3esibkith.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cydrdaja.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rvhiizmm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwvdqxl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dhfeljzk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrojufsa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uwqbaene.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xccfyarp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ddlwdjgm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gvhvphrc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3einnddit.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3osvjlwbr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wqmkrbrp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ehookmty.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3enezrgim.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eiodtmwj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fxbndfia.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ansaefzw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3slgaaqcl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jdwliudc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrmnfnd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fplieuwn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjpqtb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ucxqgxhr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ocltmauh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rtgsopfl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsizliuw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3srdazyzo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aauylipi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3oibeyidg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3halwwmvm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ategidkh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dhyxropx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgzjcnh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gauodxlg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yrvpkizn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ennbrdcu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvwmodyh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cazffhzn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmandxf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3crihfspe.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rfxsxflz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mtqazjju.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnmlqkim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3upiersdr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kxhqcknd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vnwqjtgs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqhysta.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cedhlkgq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yaoczcke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sldgtnva.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3movfvxfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kkggyqpt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jxsrhvsp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnjsbor.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gtetyyqd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sjhxzfaf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3etnqjrws.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3owjiylvu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3amseasam.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qzfrkcwf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdckwibx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qevkzaic.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kegftbdf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fbaoimak.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxrmzziz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lsomrlac.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3blotanqj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mtlfybfw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ylqoxopt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfjashlc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kktuxhjy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pogctich.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wuhhehpi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3joowcway.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fqxldfxl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cedrvbuj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pjwwwkof.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3llwsphpc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fmtxjvtm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dxrtnihi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlfisrp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzoabmxg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xirangfl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qtzkptkt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbaofjkj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qnmjjrkg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lconthnk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pkpwfops.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3diqlqdzj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmxcotu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plrmwpzt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qjlucbon.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aqikqbux.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvsmva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qcahmxny.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gmhpvqoh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtozwkx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fmzuvkmi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kuivhaul.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kwdqzwkc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vtjywgpx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vdqpeexg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gkpnlyrf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dezalhvf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hprvbnlj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bngjltaw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3itnmflkz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dotqxklp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3uhiduema.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hpcvndxy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cqirgoqt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qnhujlpj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bmrjffde.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdbbmdzx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ifnjppak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hexsbgar.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqvrfgbg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gdhiicij.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbosmstn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3twcvnspv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mrhmsoto.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3devtwmtm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nzmnbnfv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tawlyuil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wjcijpty.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ckrwtclx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xpwulfyw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3puigmmhy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tykadkch.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eiawgpcl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lvaptaij.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtycyfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vlhrbmdo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uyilvivs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdpfyfm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3slffelaw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gmksvtto.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jugsqmzu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xmkjbupq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3awfovykx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggdacmyk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldguuytm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ibqsowku.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jjagxefp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bksppunn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3elqdhhml.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3asjsykiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zopdbtvn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nqfrytfm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aooxpeti.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ooholtdm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjosgjv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aaccdwko.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzpzgvkr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuuhmkw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnavapc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwheqca.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vwgovpbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkspsndg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3reanrgxy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzpznphy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gojppjbw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bdwupbdh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpadngc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sigwdyds.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yuvtnadk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vbfxfvtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3afbgufxl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kroiyexy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3glotklku.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3emxiwljj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3upjspvmn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tqfajvfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3drsemjkp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjorqpo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tgqueubp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cjsdhoih.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qnxmmgrj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tazukcax.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wexzuxvw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ntpuaqtp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3owwludrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mqjcashb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lachulon.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ktfrqwhx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wceohnah.html


<!-- 参考信息 -->