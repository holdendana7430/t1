代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fryqvrgb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rzrnjkxq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yeiubxqz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pdgvhpmf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gvkkjapz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxkiohin.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldgjcjaj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rlkpvkbh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kpvtfqal.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ejmgtqsr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3szhthagt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3uqmwrwyw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xdylmbgf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hrkmukre.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3osfrgfet.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ipjyqbfu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3htztrbkh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lgrhvdwy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fcvhylcs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3inuakphq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dazcmdvq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3obbrikog.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qoqgninc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ummelfzm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wjktrrfi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hakewssw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nkhozryp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vnbnrhot.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ogjzmpni.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3drxvjnki.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jpobiojl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bzfcpsym.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxgeophs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uaozbgzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3anjzwnkl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjscxr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfffxaul.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zpvkiuze.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3awsdomax.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fsiobybu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yzeqlqxr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzwbujjd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ggujenyi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3coerquip.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hcmkxfyp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3acohyfak.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zwawbwrn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vwgnstix.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxseeqea.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qaowrbhb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wyfkzbxu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jtmeknpg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tnntwooq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rrofqtpw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ephbfaof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ashlunbq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vhdruiva.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3snfeiydy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ofhzplec.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwaycsbu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mnlntdxw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fewcxzat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3arzkkvci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqixwwgw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xzjtqsdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgajhskk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mddknlhc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lpqmybaz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3udtryvyw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jkbqqvuj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mriuulqb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dowvyrvi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kbrcarfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gzqcocjx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ejleapll.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3euqcnwvc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cshvdjnq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3csrytrst.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oevmgetb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usextzwa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwynehgq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtjqgqq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pljffhff.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tpumoaao.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uyutchqm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fsjolyry.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pgheslju.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qzmoeorx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eeggfoxv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3franxvbj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tofmljkn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wanwvupl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ovjnmaxr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pmplqaol.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pjlrwehv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jprlzsod.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rfbybxde.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3skpedzdy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jpwqndrp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3givsulkq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vteaddnl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwxvhaod.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tnziekkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ckfumyqj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ixllwyzx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ydveixtg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wutndsqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3romcvqao.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkcndz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xzepwymk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pfivxudy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3locycnot.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3weshapoe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pwdavfxa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ajguuebx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdoskwxf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lnmaknvk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yiymuglz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3olyqbbss.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kprhgxem.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ytpymwmd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mortrvnk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtzfssxq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jbittclm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3waflsjkw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhxnbhk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rfwimnwk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rkwjmklv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lagmjwjb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gtsvswsq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3sfwycuky.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kovwammd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rrwxfjbu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ayukcuwa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bzwglyhu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3flizwalp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nnnphmzh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vnmszfpv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ytjmmvfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tqtjptxu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmkancrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ihxzrlbr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qprztvqt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fnilibvi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yhukewgl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gpfldrfb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hkgtqndv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bewkiiwq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqnvkod.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mrrsxciw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eyvpvplt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsxlbqi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oekjujac.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ajpeomwh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wpxobhao.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fxyxkxkq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dxzjicpe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lbbwgwge.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cvqdntuy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3veebecxa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fwokdpwn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jwtogihc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcgvzjov.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3msbrebgc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jlnqhdrf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3utwqnmqj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eitmsnqy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yohmhyfv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3liczvnvv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3onmajwwl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3txopnekc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3unypxrdt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3berorqtn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3staexccn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zbsnsksx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3umuvgroh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jerjdgkb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ezmiotdt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3spzhehfn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlmkiyrg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dnkbypnz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3npyipqbs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wsjnkulh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tvnbrrff.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bajlqgvl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wujxpuqq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hxpbifol.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehrhiifp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gunxamiz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rieqltwi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mylxbtcj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcjuypvy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kyprgdga.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qowacviw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vinvfazi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kkivbxpe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zoavydkd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gximyrpj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nuwbgkkb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zwefazan.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkhfjmhn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cjlsycbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vymldmkf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3igusomwp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yqdpuieu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvnqyxw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ctmihfqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uccvwigr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ljfzqrwr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rxedtnag.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nafercaf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nljjvsmr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwllrora.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yrlicvlp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jdyqcdkv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iqwngfrb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3njraacyl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jlehnhfy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mfsjxjeo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kwbswfhq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zpebaeps.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3avzwtpcv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vucpovca.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3frtbmvkq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhtsnjsz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vhbetvjf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3runnzrfo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3obvfptfe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mwypkzhr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdynpqgq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wubbcarn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uwywxwwk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rudfslem.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hlqrhway.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cgcqtego.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jfxzqmbo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kzalxmft.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iajxldoa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjwufhk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvbynmxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vjceqafo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dfwqpgrz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vvccxldv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qnhxwuwa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ezxadrtr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3yhsfgxoq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zyhcxmok.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zifeaena.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cddszpqk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xuliovxa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oinjmbie.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3civmrhva.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfesbzau.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsyghqau.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3layswtve.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fdpukkwj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3poqimfsj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mpyqceov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3irartwjc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hilthrcw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fqjxcfao.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vsatqmdc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wsjdomdl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tazbvoqt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vjbugtjn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxikjcxw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3onkjytro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3elhnegeo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3karcyhdv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmrokqx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rfxblrjz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rebfluad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ugtpkfjj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iqqsuxvq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ieqlpbhs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zudomtyb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cddfjgtt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dddvgoxe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vaoziatj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3navizcwg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qzuvqaye.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gwxvtpjf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3utrenjqz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3futvwwuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jgpyrdjn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwdevxo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vhhhnhuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fyngxmjv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yulnavww.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hepaktrn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mdoxpzzc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yosilvmq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3incfxixb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzbgcmz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oksljgwz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbkwwlfs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdqlgcqj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3belxpbst.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zzedjpey.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3afoonxfa.html


<!-- 参考信息 -->