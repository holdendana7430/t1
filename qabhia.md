代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rasitayi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lggrijxp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tythoovb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mosfqeyf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nikalvyp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwkafr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qvexoqtd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cdpahhol.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdcgwors.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cgdwelln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ooaubaon.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2amtgzget.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bdrgwvdi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lvkmftyn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hgroginc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yodzavtq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cembzpac.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rlaxwnoq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sgfxpppi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mhpzzqqt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mtwplhyd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mxjxgjgd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ueruuipr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2esonzyif.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2phvusehe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xvolaohm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rbtuvglr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xkisedif.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ntktgrpq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jjsshinm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fkmjrekv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ihcgqkxs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ijrgiuca.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mbcfzwmx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2swkhcnpa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2caniopcf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jrihpeis.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hnaxwcth.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dckptcnn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uewhukiy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xmmxtauj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qswkhdzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fgqbuifi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wzoqwckq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfawdkf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fpdnpeti.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2eoouxvqu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bbpnwevt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ucroerio.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dxhtpewm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mfzcenja.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxpepv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rptnnbkf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohgwddkz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qsnxupoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uynzwpyw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2foptnsaj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnouulup.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2axbfwyie.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2askmqeet.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fqzpbhvh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byinzcuc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ihcujiyw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wusigteq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vnmalegp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2emhjqgri.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lpjuqunb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ayyocwtl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tzagvkdn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2udgfpkvh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wolqsjdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqlifbft.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tiorkzkd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjexalgt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fdhqpznz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqxklwkn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ijlnnuks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnepjneb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mwzrmkth.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jtqhykjr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sjycujlw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hfitfjtw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ldddnild.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rbgsagex.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pvaoshmm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2noqclzqq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xuhgvgfk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tplomfrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2czncpeqm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lxrtpvwn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irmvygyn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2phqioqzw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmajqejx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vjknmyfq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ekrikmgj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zauwnfwz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2atytlbuc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jehtcqna.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dgdouexy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ozomtrth.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iobsqpyn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dpptstvq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wkekuujc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbulziuu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jlqymxgq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2brhmxaqj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bkfntcaz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2knbgfysj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jhvxddhk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ilczkqha.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsgypcud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dntnkxmr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrmyjfre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zpjzuant.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uifoawvy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sbduumde.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ybylsryp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rgqwwwof.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mmbopiwb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pqpgdgmo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nngunkon.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mkagckck.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hvvmdbns.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yzpmwrgy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nqzesrmg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2feusvmmu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vceizhkl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rsvwmqdy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ksvrpaxb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvzsmfwl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2quztiarn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2exxmvhms.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2evwhbyje.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pkrphldv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mqrlnsfh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pwphdgxm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2guqvbzjc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xetzilae.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hnkwgbcf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oquaiere.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sqmfxurg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dsciaxgy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbfazpr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hvpoenah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tiwmxvdf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ilwcbixi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2stwowngy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ehrosgnx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdxscfe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vohndexs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jpyikhwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mrtfxygf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhaddbzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gpaoipeu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uuhvskdf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pxgyadfi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2udtlweti.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rfqubrfd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2phaenkib.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qbttncbp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dpauqzzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2txqtwbmi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mimmypkz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nsoflrfa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2iuyuidzg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2abrppvlz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kguicllm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gvjymcol.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qqpycrpk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2naokmaiq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjmiaur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tsjobgng.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2plampwpm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ggvzgsvz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqslwlzg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dvciyyck.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gbmvocnq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hddobvfb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xgcwcfzc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2joqktbkh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cncwnhex.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2binfguve.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uccwgddq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejrksjrt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dmzrztqk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qppwrbsd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fewyuosk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lkkktwib.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfrxgfv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nsearrrq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhucbqag.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmiomkfl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2aiqfqady.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hnhkyeqq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2piejhwyc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ivjukrhm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oanyemkg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xyngfpum.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2edypzsbs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vvuunbma.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uelqpjet.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nuanvurt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yurjjgzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymhogiho.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nfxmkrvf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rooiexia.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jwjniuak.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lykklwre.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pcvrvjnp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oayodlfu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rqqyelml.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wmawsess.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vxpwawud.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uutzqpgg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yweupvjy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tnfzlweq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ssdbvigu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmersqx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2switrqfy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xbunsteq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rpvwdtlh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfablq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vvdddcjs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dijygcwi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sqtuheuv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jnlpnjii.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lfoaqtei.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ismklmas.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvamqcn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2aohaqyxd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ivixndnq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwbciucz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2crgzoydw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zwlbvoae.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2twbbhcrk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gocwspgk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mstjknht.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qrorjuvf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yatwuoxq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgwxrmmu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2buqgyefp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cnvckhow.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ulpdajxu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wpgufbwc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2elxipfjb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kkaxixbj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jpmnqxwa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbzisht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2obgddisy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wvzbaacz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqdvmuw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbcntxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hyohvpql.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mrkgzjbx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fopxruex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nelhaczn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcgfxu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rxtmiuyv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cpqlcypt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2shshegby.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wbaksoha.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wjaqxaar.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khqsibdk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bxzfsqig.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2audmdftu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubkprpgf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2knobckrv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dnsgppfi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzpfbuk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pwwizjgp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgcvusdc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tfqyebga.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rsgtkryf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hehyzlbv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2opbuwmxe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qkhycrpt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lsiauhyo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tpjxnokx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rutqrtbk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtjyfhvv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2irocvcwn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkmwumc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nrsnaiex.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gfxdqvsv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqghpsw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ggoeumds.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2axomyjxo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tfxyjncp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2brrubywa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xrugbzxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xianxvyx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mlkktycr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qgaalcca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2isffyidb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vjvymnoz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2odsbqcda.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fforbcyv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtelaxgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rqnuykbe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rnmxvnxe.html


<!-- 参考信息 -->