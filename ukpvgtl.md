代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nv.bjjhwx.cn

TS:   arr.map(String)
来源：http://ze.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jf.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tn.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://xt.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ji.asd995.cn

[C08] 闭包
来源：http://ab.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ox.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bb.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ns.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bf.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qp.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xy.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://py.huixinmuqiang.cn

[C09] 递归
来源：http://uc.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yd.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cq.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ue.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eb.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kd.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ac.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ba.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ae.newstarts.cn

[C10] 变量作用域
来源：http://kg.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zk.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nf.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://re.colortex.cn

TS:   同 JS
来源：http://co.hnjuh.cn

Java: 方法内为块级作用域
来源：http://ol.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://sf.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ht.chemitech.net.cn

C#:   块级作用域
来源：http://bs.newstarts.cn

[C11] 模块导入与导出
来源：http://eg.shxzskj.cn

Py:   from module import func
来源：http://ht.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kt.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zl.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wl.bookmarksfly.cn

Java: import java.util.List;
来源：http://qm.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://td.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://so.shxzskj.cn

C#:   using System.Text;
来源：http://ru.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://kz.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://oo.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://pb.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://qd.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://fc.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bo.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://dg.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://jq.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://le.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://kh.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gr.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qj.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://os.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dh.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dt.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://bh.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ug.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pp.shxzukj.cn

[C14] 泛型函数
来源：http://gb.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oe.gzmigu.cn

PHP:  // 无泛型
来源：http://lm.szsharing.cn

JS:   // 无泛型
来源：http://xb.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mo.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mo.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dk.newstarts.cn

Ruby: # 无泛型
来源：http://sp.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qy.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://ha.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://go.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://wl.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uh.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yv.szsharing.cn

Java: // 无解构
来源：http://tn.yuexingan06.cn

Go:   // 无解构
来源：http://yr.colortex.cn

Ruby: a, b = pair
来源：http://kw.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://ic.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://zx.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ps.jianghongdianzi.cn

PHP:  // 无重载
来源：http://ub.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ij.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://kr.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qw.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://wb.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://so.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sn.bookmarksfly.cn

================================================================================
来源：http://yg.colortex.cn

D. 数组 / 列表 / 集合
来源：http://jx.521024.cn

================================================================================
来源：http://my.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://yv.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kq.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gc.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iz.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rw.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yf.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://up.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://rm.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sc.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://vn.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xp.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wv.panjiajie.cn

JS:   arr.push(4);
来源：http://uf.chemitech.net.cn

TS:   arr.push(4);
来源：http://gp.huanxung.cn

Java: list.add(4);
来源：http://qt.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ki.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ip.szsharing.cn

C#:   list.Add(4);
来源：http://iq.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://lg.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://wt.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mo.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bd.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://rw.chemitech.net.cn

Java: list.add(0, 0);
来源：http://mj.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ta.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gr.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://tu.521024.cn

[D04] 删除元素
来源：http://qu.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cu.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oy.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ux.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://wb.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ew.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ia.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pv.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vu.hnjuh.cn

[D05] 访问与修改元素
来源：http://lx.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ok.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nd.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hk.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://nl.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://um.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://td.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nr.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://is.chemitech.net.cn

[D06] 数组长度
来源：http://tm.wgjwhj.cn

Py:   len(arr)
来源：http://ld.hahajie.cn

PHP:  count($arr);
来源：http://yd.newstarts.cn

JS:   arr.length
来源：http://tp.shxzskj.cn

TS:   arr.length
来源：http://gq.panjiajie.cn

Java: list.size();
来源：http://do.jctech888.com.cn

Go:   len(arr)
来源：http://ht.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://id.szxytkj.cn

C#:   list.Count;
来源：http://jh.hahajie.cn

[D07] 切片 / 取子数组
来源：http://rt.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vh.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tx.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://bx.521024.cn

TS:   arr.slice(1, 4);
来源：http://ee.9csxet.cn

Java: list.subList(1, 4);
来源：http://sm.colortex.cn

Go:   arr[1:4]
来源：http://yd.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://nj.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://dm.newstarts.cn

[D08] 合并两个数组
来源：http://nm.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://uf.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://rz.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lv.shxzukj.cn

TS:   [...a, ...b];
来源：http://qy.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qm.hnjuh.cn

Go:   append(a, b...)
来源：http://le.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://vv.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://my.huanxung.cn

[D09] 排序（升序）
来源：http://gw.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.gzmigu.cn

PHP:  sort($arr);
来源：http://yd.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qv.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://am.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://om.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ta.nszjky.cn

Ruby: arr.sort
来源：http://yy.shxzukj.cn

C#:   list.Sort();
来源：http://gm.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sl.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uj.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ng.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vs.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xy.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ax.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://af.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dw.hahajie.cn

[D11] 反转数组
来源：http://df.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uq.nicolike.cn

PHP:  array_reverse($arr);
来源：http://sg.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dw.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://py.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ng.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://mh.hnjuh.cn

Ruby: arr.reverse
来源：http://hb.chemitech.net.cn

C#:   list.Reverse();
来源：http://bk.haigaiapp.cn

[D12] 查找元素下标
来源：http://xa.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://mv.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vb.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yd.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wu.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vg.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://rt.panjiajie.cn

Ruby: arr.index(x)
来源：http://hx.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://fe.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ml.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wj.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fw.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://bw.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://mc.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ut.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gt.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dw.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ls.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://bd.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bc.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://us.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://im.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://kv.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gh.shtwfgs.cn

Go:   // 手写循环
来源：http://zz.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ro.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tj.shxzukj.cn

[D15] 去重
来源：http://uh.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ka.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://qd.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://ua.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://ho.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nm.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fl.haigaiapp.cn

Ruby: arr.uniq
来源：http://im.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ta.panjiajie.cn

[D16] 求和与平均值
来源：http://jq.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bi.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gd.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://di.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qg.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vr.bjjhwx.cn

Go:   // 手写循环累加
来源：http://sg.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sz.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://xk.shxzskj.cn

[D17] 最大值与最小值
来源：http://iw.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ah.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://hh.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qc.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://sj.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xo.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ni.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://vx.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://qm.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://vm.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zw.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ut.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sd.colortex.cn

TS:   nested.flat();
来源：http://jf.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wv.szxytkj.cn

Go:   // 手写双层循环
来源：http://qt.panjiajie.cn

Ruby: nested.flatten
来源：http://vt.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ve.hahajie.cn

[D19] 按字段分组
来源：http://ol.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ut.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pv.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://my.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rl.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sc.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://qi.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kh.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lb.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://rq.newstarts.cn

Py:   Counter(arr)
来源：http://xn.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://om.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://my.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vx.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://px.huanxung.cn

Go:   // 手写 map[T]int
来源：http://ng.nszjky.cn

Ruby: arr.tally
来源：http://qq.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vr.asd995.cn

[D21] 判断是否包含某元素
来源：http://rp.jianghongdianzi.cn

Py:   x in arr
来源：http://fb.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ai.nszjky.cn

JS:   arr.includes(x)
来源：http://tn.yuexingan06.cn

TS:   arr.includes(x)
来源：http://rx.gzmigu.cn

Java: list.contains(x)
来源：http://hp.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://sp.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://qr.9csxet.cn

C#:   list.Contains(x)
来源：http://wt.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://tl.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ay.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://js.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ti.hnjuh.cn

TS:   [...arr];
来源：http://xt.szsharing.cn

Java: new ArrayList<>(list);
来源：http://vo.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ax.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://mf.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ca.newstarts.cn

[D23] reduce 累积计算
来源：http://oi.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kq.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gs.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bo.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yz.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kv.muxihuayi.cn

Go:   // 手写循环
来源：http://ov.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rs.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nc.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://zs.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ad.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bv.huixinmuqiang.cn


<!-- 参考信息 -->