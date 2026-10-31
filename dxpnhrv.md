代发 wailian999

Py:   return a, b
来源：http://on.9csxet.cn

PHP:  return [$a, $b];
来源：http://od.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cg.haigaiapp.cn

TS:   return { a, b };
来源：http://kv.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bx.huanxung.cn

Go:   return a, b
来源：http://vg.jctech888.com.cn

Ruby: return a, b
来源：http://qg.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://nz.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://oc.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://dd.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ui.asd995.cn

JS:   const square = x => x * x;
来源：http://vg.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://hr.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pe.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bm.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://tt.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://aq.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://wa.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oc.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eb.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qp.shxzskj.cn

TS:   arr.map(String)
来源：http://pw.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rq.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ex.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://rh.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wm.chemitech.net.cn

[C08] 闭包
来源：http://pj.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://da.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uk.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lo.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bd.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ax.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pl.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cl.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ky.muxihuayi.cn

[C09] 递归
来源：http://dy.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ad.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dn.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ig.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ti.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gl.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iw.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://op.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sn.colortex.cn

[C10] 变量作用域
来源：http://rm.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sq.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ih.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zb.wgjwhj.cn

TS:   同 JS
来源：http://qi.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://nc.nicolike.cn

Go:   花括号块级作用域
来源：http://ke.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yx.9csxet.cn

C#:   块级作用域
来源：http://cb.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://rc.shxzukj.cn

Py:   from module import func
来源：http://pi.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ho.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dt.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vk.yuntaijiaju.cn

Java: import java.util.List;
来源：http://zr.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jh.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://an.muxihuayi.cn

C#:   using System.Text;
来源：http://bk.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://tt.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ze.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://du.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://pa.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ot.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ud.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://qy.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://km.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ro.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://yl.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jl.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://co.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ts.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sm.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fm.nszjky.cn

Go:   func add(a, b int) int
来源：http://ms.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nf.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vu.jianghongdianzi.cn

[C14] 泛型函数
来源：http://hz.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://do.szsharing.cn

PHP:  // 无泛型
来源：http://zm.panjiajie.cn

JS:   // 无泛型
来源：http://od.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zo.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bo.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aq.muxihuayi.cn

Ruby: # 无泛型
来源：http://sx.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bx.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://zo.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ey.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://nu.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jt.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fs.nicolike.cn

Java: // 无解构
来源：http://mz.hahajie.cn

Go:   // 无解构
来源：http://cd.nszjky.cn

Ruby: a, b = pair
来源：http://dx.colortex.cn

C#:   var (a, b) = pair;
来源：http://nq.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://gh.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wi.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ox.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eh.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ta.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ab.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://rg.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://xq.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ek.shtwfgs.cn

================================================================================
来源：http://sa.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://uf.colortex.cn

================================================================================
来源：http://lj.9csxet.cn

[D01] 创建数组 / 列表
来源：http://ep.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nd.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://im.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lc.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ws.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zi.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://sj.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://pj.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://am.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://hx.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nx.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mr.shxzskj.cn

JS:   arr.push(4);
来源：http://qb.shxzskj.cn

TS:   arr.push(4);
来源：http://iv.hnjuh.cn

Java: list.add(4);
来源：http://kk.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://wp.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://wn.colortex.cn

C#:   list.Add(4);
来源：http://hr.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://hw.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://of.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zs.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bw.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://tz.shtwfgs.cn

Java: list.add(0, 0);
来源：http://zg.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iu.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vb.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://gl.huanxung.cn

[D04] 删除元素
来源：http://oq.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ed.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qr.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ce.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://rr.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cw.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yl.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rv.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sw.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ri.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xu.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bk.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sz.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ac.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://ew.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://sb.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xo.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ye.521024.cn

[D06] 数组长度
来源：http://rx.hnjuh.cn

Py:   len(arr)
来源：http://mj.9csxet.cn

PHP:  count($arr);
来源：http://bd.asd995.cn

JS:   arr.length
来源：http://mb.hahajie.cn

TS:   arr.length
来源：http://lt.lnxyls.cn

Java: list.size();
来源：http://qv.hahajie.cn

Go:   len(arr)
来源：http://fd.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://hz.muxihuayi.cn

C#:   list.Count;
来源：http://gg.colortex.cn

[D07] 切片 / 取子数组
来源：http://vq.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eo.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uf.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://dj.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://yh.hahajie.cn

Java: list.subList(1, 4);
来源：http://rh.shtwfgs.cn

Go:   arr[1:4]
来源：http://nl.szsharing.cn

Ruby: arr[1, 3]
来源：http://sa.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://bi.hnjuh.cn

[D08] 合并两个数组
来源：http://hz.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://pl.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://fu.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pr.chemitech.net.cn

TS:   [...a, ...b];
来源：http://nu.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qj.521024.cn

Go:   append(a, b...)
来源：http://hq.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://ti.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://jb.wgjwhj.cn

[D09] 排序（升序）
来源：http://zl.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.nicolike.cn

PHP:  sort($arr);
来源：http://tc.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mi.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nc.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xv.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://me.szxytkj.cn

Ruby: arr.sort
来源：http://vq.newstarts.cn

C#:   list.Sort();
来源：http://kh.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nh.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vn.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fb.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fj.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rj.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pv.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bu.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://px.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://js.shxzskj.cn

[D11] 反转数组
来源：http://yz.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wj.newstarts.cn

PHP:  array_reverse($arr);
来源：http://cm.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vu.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://yf.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ro.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://md.asd995.cn

Ruby: arr.reverse
来源：http://gb.shtwfgs.cn

C#:   list.Reverse();
来源：http://vw.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://wh.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ya.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iw.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pq.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jd.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tq.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://ma.521024.cn

Ruby: arr.index(x)
来源：http://cn.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://si.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://vy.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tf.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ux.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://id.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://nh.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://de.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wi.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ef.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mq.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://qt.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mi.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ne.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://gw.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://gn.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uv.nicolike.cn

Go:   // 手写循环
来源：http://mm.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pf.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nh.colortex.cn

[D15] 去重
来源：http://cq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qb.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://gk.nszjky.cn

JS:   [...new Set(arr)]
来源：http://mj.nszjky.cn

TS:   [...new Set(arr)]
来源：http://zu.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jo.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bs.panjiajie.cn

Ruby: arr.uniq
来源：http://io.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://gy.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ah.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vg.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nl.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ar.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oc.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mg.gzmigu.cn

Go:   // 手写循环累加
来源：http://al.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jm.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://aw.newstarts.cn

[D17] 最大值与最小值
来源：http://mn.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://tr.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://oq.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dr.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://pr.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ud.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ja.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://hv.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://sy.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://wa.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rq.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ao.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hb.haigaiapp.cn

TS:   nested.flat();
来源：http://ob.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ug.shtwfgs.cn

Go:   // 手写双层循环
来源：http://pt.shxzukj.cn

Ruby: nested.flatten
来源：http://nj.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qe.huixinmuqiang.cn

[D19] 按字段分组
来源：http://kk.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://li.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wm.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gg.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ji.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lq.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://jd.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://is.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hj.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://jf.shtwfgs.cn

Py:   Counter(arr)
来源：http://hn.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ky.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dc.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gl.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://em.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://ix.wgjwhj.cn

Ruby: arr.tally
来源：http://oc.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mb.nszjky.cn

[D21] 判断是否包含某元素
来源：http://dx.yuntaijiaju.cn

Py:   x in arr
来源：http://iy.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://vi.huanxung.cn

JS:   arr.includes(x)
来源：http://ob.jctech888.com.cn

TS:   arr.includes(x)
来源：http://pu.shxzskj.cn

Java: list.contains(x)
来源：http://iz.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://it.nszjky.cn

Ruby: arr.include?(x)
来源：http://mb.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://tl.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://vv.yuntaijiaju.cn


<!-- 参考信息 -->