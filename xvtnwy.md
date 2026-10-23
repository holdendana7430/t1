代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jsuluwjp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yxyauspl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bwgyppyg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3eshzpmhp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bmxxlzpg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwbtoyc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3txmuqzpl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jwkshgst.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwexrny.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qemwsbyf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvdnmcq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jjbvmniz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xxryzvnl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mrunlpos.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uvcbgwcx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hprlqxpo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xcbfaadh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yrttnfxv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sbpzwipy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mdmduufa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3otnrxpql.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3srarzgdw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ithzvhmb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3iwumtzzs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ohuhnfdb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cglcsmve.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tfqquubk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3aamvqdme.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ekvosiym.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gchqimph.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wyfupvif.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dloeqoby.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3otppmupc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iprvpxtu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kfjpcarq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bafbcdjo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3plqhyfhr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3pbayrqye.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qqyfxvvf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kzdiooxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hvtinbat.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qftyawbf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ejwjqfck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ovpssinv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgginrwv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lbnlhbyw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wvludokn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhziabd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ismztjxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ioctishi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oavuoisn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tbktdsvl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sdrstiqf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfwrylh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzfzcnp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zlpkmzky.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qpvegftr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3szuaemjl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gqcnkwhq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vsuushwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ojmtvnva.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3haqzgenh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qeptilrq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3crmshyoz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cpvzbzdc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wtapojwr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wzitfanq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ovmvejsl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hpmfkdxo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3iwlgkecm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nbprddol.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3adqcjacl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nwzezoeb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pqomsxkh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjdpwcbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mziwumip.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gnrofzuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mijqhvap.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xfcxprml.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3imchhkus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fcagsvom.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fnlkvptw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nuwxopfc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hmebeprt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3flnfiacj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vqynrnag.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3udxttwtx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gghzkcye.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3guuspdri.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xnglyesl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wfpgmzhk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3elowigtr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3urfqukyr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cwtbcicr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vphwobtv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jzobpdrv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mtnvdxib.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3irleskse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhsjthwh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xaiqebjn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxludcbj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqfosrp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ebhogbwp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbzbjth.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vkawbpzl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mnmqhiij.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tdynoszd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kwwryflo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vhrtdrmr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iufatbhi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpwkjmgv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wugfksyc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eoatgyon.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nuprxmrq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3refzckre.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qwkcmvfu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dqcntmfg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jjvwmyii.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3svmsgtqc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zoyosguk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gmoxqvlj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jooapcro.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qxewspkl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifaihjxr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awkoemvm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tnwfqxij.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kcvvlgbg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cuoiskqv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vmdaohrd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrocyfyz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bfeulhpe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xwjmdata.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ygybitsj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pcxriund.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jralbrth.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3heucgrjg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gvqvmblp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ddcfxprh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sqmaxepd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cqtmpczu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kcjzkxep.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rixlurpg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zjtjqrux.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jwswvfsb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdtuxn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uktthbun.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3icecdxjn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3anzrlirj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ehllyhrm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3skyewuku.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qblxvtaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iyfhpfhf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tedtgyxv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zehbapsd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vszvtpbr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3atntgzue.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqxsovem.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3einhkgax.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ahjzgjak.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eerhorcj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cslewnna.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjfacvw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3scrtlowv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bhrbrnqt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ziwcgdzp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bgsiaoje.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjturjw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pcbmmfke.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rfoljsiw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ncnwmoge.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3utcxpnat.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tnlqqily.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zgjaguya.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qqiamucw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nllzzfyh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rcecpnum.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zrbvcpkn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qyuidypm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lobqtqyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cholymhq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uivtfuys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhuvygc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3exkejuvx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3notlvvqn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gtwjqlnd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dycbvpiq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vcazlbft.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qguueatl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vtiqddvt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjeuilv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgnvxtgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgsbnetm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gagxoqee.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wbroesod.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsgynwxk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3clmkeqzy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hzdllwbf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uekvxydq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nakgamdt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzjsmlv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wvldxxmj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uctqakir.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yzvtttpw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3trikwclb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3aqrzlyha.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hugovika.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3foyeqczh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pjrbkgat.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gmegpiox.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3utskixor.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ltvvgwwo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hcvdskya.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfktegit.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vljghfyc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3camdxnwo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxqctdqx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lcyzwdzs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3prktsoti.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wceropfc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ddzuhsai.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3alrxpvjs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pihujcaa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iunxbcob.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpghsycj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbnvdghs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnfkowlb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bvvtpjyp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mpvprxxs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgllvjjz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wkybioor.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3esrfeopd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ybkcohgh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ekqlwddp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzsywem.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3btutntol.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uuypwvsg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3iyqmqexk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3knxukoye.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3njmuixos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hrepwryc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pkojepqn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urbfxfig.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zvrufvyt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3orvuzqko.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rltzovsa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mbktosnn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3kzeepotf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tfuerbsy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ikvhitsq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ohbvfcnw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgftbqfv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3iafjjqfz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xmynrnla.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xhwvfito.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qeelfonq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3speqlvmq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vcmzhkkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kxtocuac.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqczerjo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gjsuhojf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tabcveqt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdseoan.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kskgcxoh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmslklkb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrzlvjd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3njqiyekj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ybbhnepp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3phdlwfjw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxqxicla.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hxodifgp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcmtvned.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kbwzqogt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dnynltho.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xajnzuiu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3foiugary.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iihmfhik.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wbzigbbd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqnoucu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ufdprsym.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjqzcbzm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whbqhxcz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3frdrjjkb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3faudklyr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3radokrvs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbagsjfm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mexpqpnw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zjyvfiou.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fqmgqpcy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dtasxlxc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zxrmyztv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kfduwiya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3cgbwtigb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xqrfvbkx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jqsmvnvn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cgrhpliu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tlccqilk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ticlqbtw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhycfszx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfcxuai.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hueijlri.html


<!-- 参考信息 -->