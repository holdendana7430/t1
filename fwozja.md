代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcemjzxo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kvuomtti.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hyqikpaq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jtluncnf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vsdrjlge.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2udogzfqp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eciehido.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hseggiws.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jwuwxlbq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jhuxjmbj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qgthxsds.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rdwuxrho.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xpandgos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iwspsuhd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nopokvdx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uhvpoglf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xynfkcez.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lvltsiea.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hgmwstpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vxmyvpwr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rxixogor.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cqduhazw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qqdrudao.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wbqlxsfc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iygihyse.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vdntyiuw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jcbclofk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2aiefbjes.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fglkzzeo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yddnlgbx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pgbncezp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uvouvfuc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pdayeoov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hfbikdsp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nlpolkha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tpdcwwtn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxhwmnej.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xatzkvvu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yccsiwxp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jkksbldp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2chbgmvoc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lwodydpo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2guksnpwz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lsgwtctz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rqtcoety.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2edhaiiyn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2emdupwbx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xsvbxlev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nefggkmx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kikuzwjd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pdpvgpyh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jccpemjo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hrctdtyb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdaymbgc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vrkufcuw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2akhmsmjn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qdmpuqhb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2abhclacn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oyyabnso.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ukijpfoj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nylryuix.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rkzvtits.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vwieuxkg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cruseuie.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2efeyeort.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkbfeidx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kezmlgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfmmaglv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2oyelanps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyyfpzll.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2diirxqse.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2etqwnrij.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2simawozs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hqewljnd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ybnuxjsu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2twmbkcuh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2udaxnfxm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bsfpmwiw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qklhrskc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jjtjoqto.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qijqcboc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dypacvba.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mdqlxtnv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aoloowox.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qllaccci.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcqjwam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gzxqdael.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2llxhiedv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vljjvuoq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdlimqve.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yusviwqq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pphpzjje.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fimdbwiz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yrpznytz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ecermlyp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2pjlccelh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vidqlads.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lymtnfzt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhfxvzf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lxqngcbq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ivsoxdcr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2npzrpucg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2smkicndo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ithgvuub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ssazonzi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rkgvugik.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mnekbxlo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vkyavjdx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2evxunwua.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jkamtott.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nysvswbg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xwgacffn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cxjfbbaz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yeizvhrf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pslwrvbz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ueavfcjv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fsvltyvj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2youwffnf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjzwpotq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nhmkriqm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gvvyaecd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqgvjdfg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yxdjxlek.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dfpubsjp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zmmuvohq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tylwdaqu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2glopvycn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jkkxdsji.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ophbsluj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qztkgdml.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2plquunra.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2svhntfou.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bygetfjk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2howuzhrc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rzcaazbs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uiiohhay.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ghojhcvx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kqkvaxyx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2utfcnncc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yurakxml.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wofwwkit.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvtdaftl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yajrvbsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ulpdhunc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezymssxv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ykgwrwdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uatnoetg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jgiulaii.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dggdiyjz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ykadqqxj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gbxybfrq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ontfsxlh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2igxrwuiq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eyltpfhj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzhqgaj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iagmfxpm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ngzyinhi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lteivhty.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dnroofyr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tduxuemw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vcxvcgso.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bsivhgnb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzikxyeq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zyangwxi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jvahluru.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ujlyicum.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhqscam.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2znwyrbsx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tgdhggpw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zjzxfnir.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2cjchkfkm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fiykhtbb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eaanuddv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2etnifsaa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fxtdokuf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jlduhzjp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2djoxmbav.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2omhpmiqp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wsggtyud.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uldyeger.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hdrbishm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2npzbmgmq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxzcftbr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dkyuupuj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lonearru.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lcydnohf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnjecwaq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pznplphi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ivjlyglp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lunrtajb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrxmhfz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2koyqgfke.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yzwxpyss.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mvvddzhx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vzvdqqcp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zytipgcw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bjekjxug.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yrwqlbbl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2baczdcle.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rnhpgqbc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ptahlfjq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2owhoekjc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2roptcmxp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cgjgauye.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2etbrklxl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nkvydgdf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbbltbr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghzlugdq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzibigl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kdanqsme.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2smrcmaod.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kjffrghd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tyqkkfob.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sagurnkg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2anpgjnba.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2acechkfj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jeymqget.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjaouju.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ktjyfhfa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sdqbekis.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctezrfgw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gvxbxhvm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2glwfypvc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qapdohwv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fhzuvesz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2erakilah.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqetuxr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aiwskctm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vmfpjkif.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jqgdslkk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qsvcgyuq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcktsote.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmmgudln.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ddkjhkjt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wvsvsprk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vkydkkxx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uarxsjok.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2njaojmve.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2euquraof.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mlopnuat.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wxpmpgjh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ysqyxjmt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxkcumji.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2towkkksd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tnpocmiu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wgtqvpcc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hdfdefrq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ynllycvz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fkblhmqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kuhglarf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dapfswzq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hotpettg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rqnsvuul.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfsmnybh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byjjkbhi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbrfig.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ugxxjzxy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sifgzgjn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unaflpse.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ufcystqt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krtudkrr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ysulptti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2crjllfqv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dqydcylx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rhomfamz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2twbufvrk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2otcukkuj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2meioqeip.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gxbjunmf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yghuwivz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ynxidqeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipckrhid.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aiinyqil.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2syklfcau.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pquohxsr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wuplagud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhporhhn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qqbvlkvb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2habsvxwn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2haefmihs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljscggdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmgcyvt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2evjohyya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tzdiqyns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vbektpvz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2melprzia.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zvszasqe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kvwdotxf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ihxximsg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kcbrbcjg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cohahbdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xicjects.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yqalpngu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kaleggmf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utwafkbw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2obhojvoh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qfmpwnxw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gqiqozpk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uroxlcrm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hrccsjdv.html


<!-- 参考信息 -->