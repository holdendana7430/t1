代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3otgopjdo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jthsryth.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rluxnarb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zabuimru.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3crxpffct.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yhefxnno.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3egbeuuhf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kzypnjkz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hyrpentp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3scvnngqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bnidqkiv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3morempwy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wwghrtxt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3npoeoysr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eijtalnw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lrbqqxid.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ksmvzdkq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oesssmuc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vfsufcxb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xzkprdru.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qhsvwqpr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ekxxfnax.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqicsr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3abkdnifo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3hyifljzo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ssfsnajn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3phpunqje.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3htmkbmzm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ysszkbis.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pmamqfpi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kwxhfufb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3orsqimou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vgwtnepi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yixcjzza.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfamuiet.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fwoarmrx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lugsspvk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iluehjfb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3oojvbail.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mzlqzlax.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3llbkvyoq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ioryqgms.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3znfpkqlc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pschsnax.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcvwbfjh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kkryhawk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ydlebqfe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uptpfnge.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fivqqwei.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aekipavm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zoelalzd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ionfkcru.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cmrmxmyb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxlsttwb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3djjjdeja.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3onmjjqyl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iukqdemh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xtwswvqn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pbuedztk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ucketirc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wajxxuvu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zfzifrvu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3azmsrdzj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rtzawegh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkqdth.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kqfojgwk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kqionkwx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ctogznvy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kgpkshwe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3oqseqnlu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xggklrrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wppojkuz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wlkmwcoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfpsnswj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zwutzrvs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3whbdhdya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3crgpbube.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lvttjhau.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ciesflso.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3njhgcepy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3galxyohf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3okbfmjev.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dxzxjhzn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3orvmeeup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3djzzmxif.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ffxhxumr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxzsshoi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3btocetbm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gfiqzcvr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfspbyj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cbgqpuue.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3yqmvomkh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nzuwqnma.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kmdnjrwy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3enyusyut.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gvzflxzj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkaqmge.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqnobebw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3obguwrvo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jijtqwzo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqszrjrw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3facfvrxb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ehaadusp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwjdudpn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3evrfzhvp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vrwdllqf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tsexxdzf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lbyndszi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3icpwllas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzsnerw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uzlaxdeg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ysveavkz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fthmnmve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpkgwj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3trlidqvj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zztzyulh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xppgyrcj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bgfzgtjl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ncchystc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dajacwqr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udqvwgyb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxcdsjea.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nxuwkgvt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ipepzwkx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3egquskwu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnriufyr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qgdkcqxm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zssespaa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xhmzllkr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wicdomia.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3foinrzre.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zecmhptt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvoyzzh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3huoadahz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zmkpelbh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ldccdtlj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shbqxkdd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ftpgjoqs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nukatdtw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jkveidgy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ykrfxmsa.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3krnaambl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqzgvzho.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oviqcbhk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pahmouvy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqbyyvpe.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wqkgghio.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dqlyndll.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvyzcyko.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3piemaocy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xnxfulmm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jelwloih.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnivddnt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hlomouyu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cbnryrfr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xuabikqb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kgzqrprn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmykxvl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kvdjdebd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3edharbqg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ygbigelv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sxadbrie.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtdptbpn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nrehmfer.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gphontjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3duojajkv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3reghpcoc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nsvzvwym.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yspygjdx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3otfydyid.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhqfstdf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vmjeqjxf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fuqjnedz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lrcmpsyk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uyxttluc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xfeioazr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ywbnivku.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wijxwexz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wtgcycmr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvtlwfaj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjwwbga.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wsqginoe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fdtsjmii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uduatpge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iglyxnsu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxqunyxq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ueeekpzq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hlsmrjso.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aoezqcqg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dmeptegt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3czdkoain.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tqnxapnt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jxpqdzfq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqamtcfm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwktvmay.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hpromtjy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ccniomce.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbbvomhg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cxnrrvhu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwwchxoy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zvxpgzsr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xyyotczw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldqzopgo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bzownmdt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fyoslgjo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3yoznmynj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fecnjxnx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yecfbzvk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jshnxwpd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tfmocdor.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxjyeopv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zdpmziat.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fgserkmz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3efhnpzgu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jexoiaje.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3olthouwk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3uhdkgjrq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3iwqmjlln.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3swcsinca.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qynkfvau.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qquvfcie.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lkpdxjmy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qyeyapmw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qrtpzdrp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znupqdkv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vqdzckha.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3itzjugrs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dkopjdzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vrjudgzh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3roeajxln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhksfrp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vbntwfjx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cbxxzhlx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xtqgjrbm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cbabxtme.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhgfqqzu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vagqqpks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nxfzoisi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3aivwdonk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wtbevviy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmiytzw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fvqchueq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yzlfwfok.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfdljau.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bssfswbd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3opnthmpu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmweqgl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nzojmchw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fnebkzdt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3shvucloq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3huysudse.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uigcmjuy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3slhrifzh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hggpagtw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wsetkkpr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mxebnvut.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ougpafvz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzhctupa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqiltv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3syysxswh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnxqzzq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pakiplxf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dhjjiulc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qklgxdnr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikpzwoxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wrisjsqj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xjpkbewo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gevevixo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pyyehxve.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfgxmcl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gpvqrzig.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jetcucqw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fvfytpvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkwrzpt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwoeekn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mixcsljb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmoespvm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rfjylmxh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ckrnmqgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wnfvqemo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bikpcvih.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qfxjxgqj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmkpsd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tywgbzpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3syjohkxx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tbwebvcw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehigetrd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tttlrsux.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oldwvoib.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3orptvxmh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zlvwyqoo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ueollwtd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rryqfcho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zisggvfw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3reldpqvh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whrfware.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xfxipsji.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bliegxvm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jnncnryx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3snqniphy.html


<!-- 参考信息 -->