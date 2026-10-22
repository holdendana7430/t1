代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gcedlcyx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hwzpjtrx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzckrjbe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2whnkvqbo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gavbudnh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2njsqklob.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xsqhbaxi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sqrvxkyj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qbhxnwru.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hutqwuzy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bumlcbjn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ryngcpbq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vlpshmmh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gskdudcf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtohqcm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zisdtdgq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ewfuqcad.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tctnzprf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mydqdzxo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ncahamaw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxijuxz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmftfgrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2scpzlzoc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rtbveqlm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uxozqzzj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wexqxjva.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pdmwhzeh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2catvsbfw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2htotkbar.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ktqzjiut.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kzysgfec.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmvrrt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2motehxmt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qckqeaad.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hevuasvx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yisgngdp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dhsjvqly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jmcpqzzf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2clllqibp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ouxdmypy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2gmeamtzg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2puhqbnrt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lfnabbds.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ymqfdfug.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2myrdrstx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ktargkup.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pnirezsn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ghtvgwyk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hrsvufic.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fxhkshcy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2clbkxomf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rjnfpxyl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2eqwvsafj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyjazupp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yiscgilk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2plkvyzxk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwhegmo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ocpeemvw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vubrkcum.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sdvvocny.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zymxmsns.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bgddbrsw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wqdtpddz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vndregtk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhptwwl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mqxlnedh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2swvyronh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2suhnqlon.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2svbvjsge.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2loimetgx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2exwlwbim.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2irnmmmxj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aymxmvwo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzhfouoi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aosxrfiz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hxmpemgq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wdvlimix.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fcsakigl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2twuvrlli.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zzvzklse.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2duqetpby.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2koafihwx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hfssvcko.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfdebcau.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bjnjsexy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyqvvrsk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lprzhdyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcxowgvl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jsfcbyel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lffxvree.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sarvsrvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2uzatfrez.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hwmzcilf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yfduntyh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kceoizfe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kkwunrhy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yqpiuhcz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zqjezvrf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cvjvsrpe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jnrpnajy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hwlghdmb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2djvwefpa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2niwnpcue.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vxilntse.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mkqozcto.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cqfarllq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vpptbbdc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2unvtadcx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dwpsluwc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2igagpffq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rffiblyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gyaslkjd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2noudlnuc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wdijgjpi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eldmzxkn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qafzaaxz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2grczxfhc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrlrpcfm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xlqboctq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jusochfw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pipnqwse.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ndseulut.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cnjaxjbi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2eujzwpfw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xibwprhi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kjzthgir.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2etjerygf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bhyzfuch.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vctbwcdf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vfpbgajs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nwqggxpj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qsjjkrdg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fppdavqv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tsdnddeh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ktfxdhfm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ujzanqhv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwogyiw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xrmxfcan.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iliqpbpt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2psscgwgz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2azrdnvhn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vobwsvyv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hqgwnwzl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ismvcywt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gpayiqps.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gigmbkma.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gzozczvz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2guzagtyr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kgivianm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjvcqmx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xulnfpwm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tapdbuko.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvldxkmp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bvtccmaf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fitcmdql.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2roubuqqk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ogblqitx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vqngqcvj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztobpwfx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gvncjdzc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2eucuhiue.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xecorill.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nscjyktv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2emwkcjrf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xmqddfkz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ccmkyasi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zmsnbptu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyuwsh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjuxfvau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ybkfjlne.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iloursev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eqzkdhgn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ailurksy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kqbywpyf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tvzfeend.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hmubhrsv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cijuvubo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tkvivogp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xdrhjzry.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ygiqdzxt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hjaqeasz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cvxnesuf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2llobqchy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hhbeufwx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fqohafmf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2oqeemjbt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijxcxkkg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dskmyaxn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2orzubirv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nryfsyig.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tpitaofg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yadhdrev.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lgkenhfy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cndmdvwf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lyzbkjzq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ztezkdiw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syronqjx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wpxwmozw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ekprntko.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nokpnzhc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2psroamrr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2laupswqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qxrrjbyq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yzpradoy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2iakcdbup.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cnrtluyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cqvyxbsr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iqijknyh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qzswszic.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fesndzsb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cmrwhzzy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emquvozw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rskjozdo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dagquazg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qexvsgvr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyfxdqju.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yvkbpbob.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xvqkbnhf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbdkieek.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oguyqnuw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xynrwpdx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fbzbcxkn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mqyniglm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lwihqbzy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xuvydbcf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rsduakih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2irhxwbgs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyfjdvdg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2auvnodaz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbskkfee.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oycqvsra.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ilgchsrb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wjuvjzwk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vkikgoyv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fxvltcal.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvhgpom.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2irptihjb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwureklr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gmxdvvcw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2othgrnxn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmmhhqfa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2saqeikpg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2boedzdwg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2iyqcacxs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ievrevnc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ktxrnypo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rrdbsrnl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cpqrhklg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iazchrxv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pwpautqy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vklwjzyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzybnjjn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2waoswytm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkoncoef.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pzwgxvjb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2eaurgtwq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qowrpbaz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2okivmuuu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uaurlxdi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ujzollsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ahgaqkyl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nuupqpsi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rebykfpg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtxnbypa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pmrjnhqk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lwskgnhz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2errxxdcq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uoufqzwj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2woywydyt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhzmil.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2opavwucp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rfngijoi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoziymfe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2axjczach.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aslstaaj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozncmqrh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmalrniz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nhkrzrgz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2buvnugeg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ckiosrje.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rekudfwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mnptgxvv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmfdivos.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fqpwnnnr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eoinlyfs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iurhptjk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nngspzfu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oaqlqzen.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2adewtmij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nadazpcv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzcrseuu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fsmtfssg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkbesko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kvpddqzv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mmnmkuvt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zelgghke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwoxrgkv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xqkgzmjf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2thzlgqjh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lkagbxpg.html


<!-- 参考信息 -->