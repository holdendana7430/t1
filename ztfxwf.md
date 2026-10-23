代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3auxsqivn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kceuoser.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gefmlhjy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cqaopzih.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pdkykgau.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3roxqmoeo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibktubzl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ubzfxpqr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ggfmaxbd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycuiileg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3whqgpjxs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3reaxcffw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uvbvfdyj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3arqfkdkc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vvvpsynk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gyjvbisc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cbdzgntq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3baozytal.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoehbxnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmfgatck.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xasujilj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cksrafff.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vkocufex.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oafstyux.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kjqqfzfl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ipfijdkg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3afffskun.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kieygozz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fszfjgnk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qoemlcuw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ivanerdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lwzspgwm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tjzmtagk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tjpcospx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uoppuwbp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sovxituk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lycinngx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cthnmqwf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ysmgujtr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3frexlpcz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ncbugdhi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nshsmpzw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wiwfseot.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fqvifzhp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lzurpuvj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wtxlxyhp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwixnr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rdwzizzz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aeeurtgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kcbzbhvx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fclqmbjd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvghadsr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lupcmvlj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tzkaizbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xqxicjxp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ucgadlen.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlunbpxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mkevsixw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3blwmdiag.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uzkuimem.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lpmolpzu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kppiybvm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xcgziacn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xvngprst.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oazunrhy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hxfuvnlh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3inxszsqz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hinujszz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tobufyzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3obhupudf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nchtchqy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kutwlulh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hrafwiod.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kmppotez.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3akrgytoy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cuudzxoz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gjhpkjhp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zlnishyv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oybkthyk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulcjlilc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rgxeyeyt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxjtsgoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nyicscqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emrxhjgu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kvglohhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdpiejzw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rnswuwwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3adjvptrt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zcxqjqvi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqiqwofe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tzhszfbp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uowwbhwh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vyqitvbp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kchdiekk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mhbuknmk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bvygaopn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yjqfhqgj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3neiolhak.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3colhlklt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iahyejob.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zlpvcrau.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tcusmhbr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nvsavahv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tquglyrt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hijnjkhe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lslrhgpo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvurxus.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jnygjqzk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lubylnmu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vbzuwkao.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xbottkik.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zbdsigit.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxbyaex.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvgiiewx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzrqpxrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzyfomrj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3clpnblxh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dwustqlq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fbaysnmj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yegmqtcr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dvjlszvt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3huvyoyba.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gvgfuyto.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yudfboen.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wfbaalhq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xaiusrqp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mupfaijs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rfykeqsy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3huizqpbr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hcesklrn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hxkxonpd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3swnbdkeo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqyenlou.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ddryttng.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kfguvwui.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxewqzpz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tufrggvk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aufwdgby.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ezllwmhi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xkylznie.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ofstrtub.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fgrhusqo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ecdtmgfl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lqyiyviz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dndzvhtz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lbpkmpfo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eygixabw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oztgqzvp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3riuavziw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rkpwwzoh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rbdcsbgv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tijamalp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ttnwincw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3obapjkmu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iexebnwy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sthicequ.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbpbcvv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwnooccw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tpubfwvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zqhkegsp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3enywvuhx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jfgzicmi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dhpbbzkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pchimmre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzvbkmxv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wsiphfuu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lsrqwojz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3udjtyhji.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrixiyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tzgirpab.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vfauysjn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lvcdohje.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vfvoiuzj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fsmvtdmf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3haertnqv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xfaqdmok.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3alleodoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tczsgzzh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3poqpvcev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nrdtyjub.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qlqrmfyw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kaditzbo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erqzwpho.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3twtanloc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3knvkujld.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jwqeolgr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hwaroitu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fkhjpyfo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuoqqdir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wiyoqtta.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3abudxpyz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnkxubs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wdmemxey.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hkhscvzl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cotrtrit.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3oczlddgx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3druwpkvc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxsgfqbn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlxgbap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dctghbsh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nkifxddw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtoadiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaczrjiv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qfmkdywy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3okalerjs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lmlukvoz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ngtjxaby.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kyqdhjyx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvbzhtaw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3atdvodha.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bhebqlrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jkefiwjz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hcyclpfa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ixdimyfn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cnjrsnwe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bkhuxxsd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3htabudjj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jumekbmd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xesxywpt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ppzazuac.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jjzknaij.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ihtpyhxr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3djgjszcj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aiempboe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djcimvut.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbftkam.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gprrfgtc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3aksntphm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xmabrgjx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3idalsojn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lmqggtlh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ruuqfhlt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jcucohob.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3aavyezoe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acknnoqn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oaljyvfh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3atfltxuo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gsfmbvny.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3toyhuqpy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xooqbtsn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3arpdujmh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3akwwkkas.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tldwawjn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3elndjfzu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iokjmokn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xsxxhjbi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tnnisbwy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mssbsgmc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vwjlmqwv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fiyvmqlo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gjrdolgt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3eiwnbwqq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ggpjxykd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mlmxdhqm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bojbbibf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xbhnrbni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jgylacdz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hqurghfv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gdaqgxpx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3atbnaain.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fngfjlgw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ysjeaxkf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kexmrizw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bdzltcac.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pqkffwmw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fyarbqdf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wrclivsw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hrqgrbzq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xorlirev.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrkknlf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grnxxhdq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcjgrkt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzepcycn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxkralr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zthypdxa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wkgkcaik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3adqswnzf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3psxohjgk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3phghkuze.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fozhnpal.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sxadduuk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3neywibqx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ajrryhde.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rwjlwnyk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jrssjxuo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hbidpasp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xryxhgmu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ldcxxvlb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ejscrvsc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bpxpsyef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bzqyanar.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gbleejlj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eowwwtev.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ynzhhcvj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qawnzpyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjoixbn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtpncjx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqxgtzz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqswkvk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qsoanzsy.html


<!-- 参考信息 -->