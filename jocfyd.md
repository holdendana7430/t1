代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3epavkeyo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xirvwkmz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3horgjtgo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rvzzlhds.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3aotshtcy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jsgtjjkm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pwwigxau.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ebycknpf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrrnauf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kzfnarfa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3evenqmig.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xnsapuen.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3chhikcuz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xfzaanyr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pyspityf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3emfzjfxo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pejtrlak.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ayhxoacc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zmwjwewu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nceyhcdq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fzwerysc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3cctnihhg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ootbtnce.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jfsjeini.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hdsijnhg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xgxynfdv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kehbzhtx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dfshjlbb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tiucrgcy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3utmrplpu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mfmcvpll.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3afycmtlq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3klmxfcbv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iezrqmqy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tzszcwlf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3eeuawdtt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3skfkuwib.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rgmaydug.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jlwlmqlo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3blbntzut.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wjfendae.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xrarqljy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cngtgvvf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nebycndg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vyjkavyq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gadsawum.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3airulapn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cpndgeua.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zvbzwqdi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ngopshpc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ibiiqkxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvecaete.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3magauvhl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3acpozdvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ioautwfe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ujsvjzov.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xluwjcnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmksbo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3clfujgvo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3omxtnstn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cghymjpd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3htjfflhs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hwfggggs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tsamxmug.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hegtcmog.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3eudxicno.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fdutdnmh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xmvluinf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bqyxhhhk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfsujtlq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ywvrnygz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fqnzxaqi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vactpsra.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lobwacvm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3apouwhlb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3giytpxol.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ufnfuuar.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zfaqksll.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wejobsft.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddtydudn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3idmtmnbi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lcomqxed.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vmwfrwhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdrdgzdj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xrjdnzac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jotsgich.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ymcnavfl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tuahkqgh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oqwjgbtz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qhocklmk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3fcdgzqjr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nuupgdmh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3opdfzuzi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iatpozrp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sgdjuqaq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dxrtyphc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hrtnnrdm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hsevswyl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqczhcaz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jyajkwsy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3khjmyuuf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhbwljf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hsjwditm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cgwhpzeq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vdzjukcf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxawhsu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmiwradb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rrjrhewr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3niwukezj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckbmykja.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3znisruym.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ncsjwmex.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3otdepelf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ambbgyis.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkjpkdo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wxuczpzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ftkkgowj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wyunlpnr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3iizxalpq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qnmimdmb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sldpcbua.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3aqtpbshx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbwguyde.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ftxxijcr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3azhaofvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3djsaqdem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ergoqraa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qhzcxrtk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfhucb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3axfyuvov.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uwvpbcoe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wpriruho.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvqvoerw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uejchsbn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rczmzfuo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxxirehp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dogmipsd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfbalit.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3waqofjtf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pozqrwzd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ddujzmqe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ysiemmka.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aysywstp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3spfzoemw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3juqbojsl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3voylpzlf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qqnviolm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pswzegnv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oygrlbvk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bmumwfhq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mobeyatw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rmiymzdb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nrajxjtl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dbtqxpco.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mctrtviw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ynuhugne.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lmsvchao.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pntvpiau.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nxwicche.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3etqaudha.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3maxviezk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3crocmbcz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zuapfceq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cftiingb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpqbxohb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3djilckeg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3idzhxbfb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ekwidoof.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3afjclhag.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ekstltra.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zutqsspf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qzvwbkmz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xfolqlnk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3onnmnyea.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqbicze.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vydbdwxo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3alzluobd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3scwsgjfg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zkphmqdi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qxpyvstr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bvklvtta.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3btphzhqo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3firadabi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jqwcyqnk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dsaggine.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xcxvprpy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vptfkcsw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sauyewuu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbetotr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgpgrme.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hurostyx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvomkxz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ntzeheyk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ymjheqre.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cknoapcf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cnxiufgx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fxlqyeax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsqovyhe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ygnnjehv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ctooduvl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rgcacogf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3inzvnltq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qivdxgzw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zghgotvw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irottkli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrkmqjuj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tttxhrox.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyxensb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fmwqgqhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kskkcmgm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvabzgbx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwuvgvfc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tmuwjnfl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzhfmwjz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yslxcsen.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mxcoopuh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eznviszm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bojvvkur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fmipcwsy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lnaszkga.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uygczrup.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3limhrfam.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jjfvehsg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3emaeeccl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vegzolsn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kztnpslw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rkysenpc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3glmupwlc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pvvdagzf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qpfpixwf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qyggrmex.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3krlajirb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aujgrunr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3snsrnqru.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvwynptx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lsguqcim.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrawuqgj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3andjgjmv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jacunuwe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xggxvxdv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wmuwbrfs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3uktgifzp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pzglobbv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gjsswnos.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3encmrcva.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xkdxpeja.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lrtugqlo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3urgwgnyv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zsgsreof.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzczempc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rsdzngpg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ejzpbiit.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3omvilpbl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fatnupgp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xckmuhxl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yxhosjqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zgrlhyty.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nfbbjroe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuxeafuv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uowxmkfq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nxnxlhkc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3omxexwyb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ahrkwwzk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xzrvowyf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3eunydnwy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3eeqrqlze.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dabtqqiv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ylhnsdmp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qslxfzpz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tujhkksg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3phvanqky.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wswrqutd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtshzal.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zhhrewqs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3braaiuem.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3atvwwljd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uazhqhxn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3klqbglsy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnoidhd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3miknrfbt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ujcdbryp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vvejcvwh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hhjlekrl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3icmyilrd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vrxptknf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilvjnmde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ixucmgvg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggmbdbco.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dltquhur.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kulmksga.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nqqhdbyv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hvboriol.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3liasvuta.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wfopxqnj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qodvcyfl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kvwneoje.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3buxdpgcp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3odcdbweb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ysfnowlj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3htxsnbjm.html


<!-- 参考信息 -->