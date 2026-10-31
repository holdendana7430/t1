代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cm.huixiangedu.cn

TS:   arr.map(String)
来源：http://jg.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vm.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ya.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://pj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rj.hnjuh.cn

[C08] 闭包
来源：http://zp.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lh.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bj.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dn.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yy.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zj.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dk.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://py.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cg.yuntaijiaju.cn

[C09] 递归
来源：http://qk.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jq.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tb.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yu.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pl.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ly.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://io.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hd.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qe.huanxung.cn

[C10] 变量作用域
来源：http://kn.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xg.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dx.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xn.wgjwhj.cn

TS:   同 JS
来源：http://oj.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://md.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://ax.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wk.yuexingan06.cn

C#:   块级作用域
来源：http://jl.shxzskj.cn

[C11] 模块导入与导出
来源：http://au.szsharing.cn

Py:   from module import func
来源：http://fn.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zz.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hr.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://es.asd995.cn

Java: import java.util.List;
来源：http://nr.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ac.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://el.jctech888.com.cn

C#:   using System.Text;
来源：http://tq.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://fu.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://ke.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ec.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ju.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://cw.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ra.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://za.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://qk.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dy.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://xq.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zz.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eu.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ng.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vd.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gc.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://jf.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pr.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xs.yuntaijiaju.cn

[C14] 泛型函数
来源：http://qy.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sj.chemitech.net.cn

PHP:  // 无泛型
来源：http://qn.nszjky.cn

JS:   // 无泛型
来源：http://vb.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ub.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bs.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vn.szxytkj.cn

Ruby: # 无泛型
来源：http://so.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://av.nicolike.cn

[C15] 解构 / 展开参数
来源：http://rp.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://or.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://fw.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vs.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bm.gzmigu.cn

Java: // 无解构
来源：http://ao.shtwfgs.cn

Go:   // 无解构
来源：http://mo.bookmarksfly.cn

Ruby: a, b = pair
来源：http://tf.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://wa.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://mq.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ka.szsharing.cn

PHP:  // 无重载
来源：http://ub.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ts.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uj.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://jy.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://tm.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gr.huanxung.cn

================================================================================
来源：http://vz.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://cp.yuexingan06.cn

================================================================================
来源：http://ug.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ng.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xk.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lv.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ro.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xj.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rq.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zw.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://eo.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jg.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://cm.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ph.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://da.chemitech.net.cn

JS:   arr.push(4);
来源：http://bf.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://va.huixiangedu.cn

Java: list.add(4);
来源：http://rw.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://vh.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://if.hahajie.cn

C#:   list.Add(4);
来源：http://gc.9csxet.cn

[D03] 在指定位置插入元素
来源：http://pl.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://yl.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gh.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gp.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ta.lnxyls.cn

Java: list.add(0, 0);
来源：http://og.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://on.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ex.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://nv.asd995.cn

[D04] 删除元素
来源：http://lt.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lu.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hy.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kp.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://zz.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iw.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wc.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wk.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qy.lnxyls.cn

[D05] 访问与修改元素
来源：http://zu.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dk.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hu.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://go.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://dr.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://fl.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://ff.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ws.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cf.shxzskj.cn

[D06] 数组长度
来源：http://fd.szsharing.cn

Py:   len(arr)
来源：http://yl.colortex.cn

PHP:  count($arr);
来源：http://sp.shtwfgs.cn

JS:   arr.length
来源：http://sj.gzmigu.cn

TS:   arr.length
来源：http://sn.bookmarksfly.cn

Java: list.size();
来源：http://gp.haigaiapp.cn

Go:   len(arr)
来源：http://jm.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://yr.huixinmuqiang.cn

C#:   list.Count;
来源：http://cw.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://tw.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dv.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://br.521024.cn

JS:   arr.slice(1, 4);
来源：http://iz.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://sm.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://bl.nszjky.cn

Go:   arr[1:4]
来源：http://qi.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ha.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://pl.shxzukj.cn

[D08] 合并两个数组
来源：http://kk.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://dw.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://pa.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oc.hahajie.cn

TS:   [...a, ...b];
来源：http://su.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vt.nicolike.cn

Go:   append(a, b...)
来源：http://nn.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://rj.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://hd.muxihuayi.cn

[D09] 排序（升序）
来源：http://zp.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://xk.yuexingan06.cn

PHP:  sort($arr);
来源：http://vy.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tm.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ba.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dg.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nx.nicolike.cn

Ruby: arr.sort
来源：http://bt.jctech888.com.cn

C#:   list.Sort();
来源：http://tu.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ur.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ve.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kw.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://my.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mg.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mx.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wu.shxzukj.cn

[D11] 反转数组
来源：http://rk.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ds.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://pi.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gh.521024.cn

TS:   [...arr].reverse();
来源：http://hv.hnjuh.cn

Java: Collections.reverse(list);
来源：http://cf.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://fs.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://tg.yuexingan06.cn

C#:   list.Reverse();
来源：http://gc.shtwfgs.cn

[D12] 查找元素下标
来源：http://am.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://qh.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bm.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pn.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bo.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rc.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ij.bjjhwx.cn

Ruby: arr.index(x)
来源：http://ql.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://et.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ms.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ah.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lg.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://gg.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://nm.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ae.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xj.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vm.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cs.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://ek.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vz.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fe.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://le.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://ln.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://io.yuexingan06.cn

Go:   // 手写循环
来源：http://az.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yx.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xp.521024.cn

[D15] 去重
来源：http://np.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kr.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://bh.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://rt.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://it.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uw.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tg.yuexingan06.cn

Ruby: arr.uniq
来源：http://rp.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://vw.szxytkj.cn

[D16] 求和与平均值
来源：http://uf.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ft.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ke.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://et.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bu.nicolike.cn

Go:   // 手写循环累加
来源：http://mr.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yg.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://uz.hahajie.cn

[D17] 最大值与最小值
来源：http://ht.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://jj.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ds.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://su.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://di.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pu.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ap.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://sn.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://el.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ai.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mi.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://fe.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nz.9csxet.cn

TS:   nested.flat();
来源：http://bw.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://km.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://lg.asd995.cn

Ruby: nested.flatten
来源：http://sp.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://no.yuexingan06.cn

[D19] 按字段分组
来源：http://qx.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pf.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nu.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aw.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://su.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cu.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://ci.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fm.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qo.colortex.cn

[D20] 统计每个元素出现次数
来源：http://tk.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://cm.asd995.cn

PHP:  array_count_values($arr);
来源：http://ed.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vo.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hv.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jg.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://cn.shxzskj.cn

Ruby: arr.tally
来源：http://fv.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qz.nicolike.cn

[D21] 判断是否包含某元素
来源：http://de.bookmarksfly.cn

Py:   x in arr
来源：http://uf.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://gz.huanxung.cn

JS:   arr.includes(x)
来源：http://tv.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://tt.asd995.cn

Java: list.contains(x)
来源：http://hj.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://bn.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://bl.jctech888.com.cn

C#:   list.Contains(x)
来源：http://hk.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://xh.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ik.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oz.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aa.lnxyls.cn

TS:   [...arr];
来源：http://tz.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://qb.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zh.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://mk.colortex.cn

C#:   new List<int>(list);
来源：http://zd.lnxyls.cn

[D23] reduce 累积计算
来源：http://de.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://at.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pb.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jx.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mt.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zr.huanxung.cn

Go:   // 手写循环
来源：http://ao.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://px.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dh.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://co.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hq.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ip.lnxyls.cn


<!-- 参考信息 -->