代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://ws.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zz.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gg.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://lo.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ff.colortex.cn

[C07] 把函数作为参数传入
来源：http://mi.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ny.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://th.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bt.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://fa.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kp.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tu.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://zu.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wt.haigaiapp.cn

[C08] 闭包
来源：http://jg.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zb.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gj.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gv.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tm.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://no.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qh.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ux.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zp.panjiajie.cn

[C09] 递归
来源：http://gb.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wq.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jo.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lz.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oz.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://on.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://by.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xt.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://di.muxihuayi.cn

[C10] 变量作用域
来源：http://ue.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ls.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qz.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xq.colortex.cn

TS:   同 JS
来源：http://gb.521024.cn

Java: 方法内为块级作用域
来源：http://lw.chemitech.net.cn

Go:   花括号块级作用域
来源：http://kg.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jw.bookmarksfly.cn

C#:   块级作用域
来源：http://wy.chemitech.net.cn

[C11] 模块导入与导出
来源：http://dr.chemitech.net.cn

Py:   from module import func
来源：http://xf.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://js.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ox.jctech888.com.cn

Java: import java.util.List;
来源：http://qu.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cf.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://rw.haigaiapp.cn

C#:   using System.Text;
来源：http://jd.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://ac.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ne.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://tl.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://af.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://yv.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hk.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://px.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://gu.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zc.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://cs.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ac.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ah.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hn.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://he.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kk.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://pq.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nm.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ku.yuexingan06.cn

[C14] 泛型函数
来源：http://qb.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ld.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ac.9csxet.cn

JS:   // 无泛型
来源：http://ok.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ts.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://th.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ci.hnjuh.cn

Ruby: # 无泛型
来源：http://ov.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ba.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://xn.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mc.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://qq.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vh.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sa.gzmigu.cn

Java: // 无解构
来源：http://yk.jctech888.com.cn

Go:   // 无解构
来源：http://vr.gzmigu.cn

Ruby: a, b = pair
来源：http://wl.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://tm.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ro.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://su.panjiajie.cn

PHP:  // 无重载
来源：http://jo.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hb.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pj.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ql.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://hq.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://mk.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aw.lnxyls.cn

================================================================================
来源：http://xz.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://iu.szxytkj.cn

================================================================================
来源：http://vb.hahajie.cn

[D01] 创建数组 / 列表
来源：http://cz.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rv.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zy.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zr.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lo.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uv.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://cf.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://bi.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ep.9csxet.cn

[D02] 追加元素到末尾
来源：http://gx.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://af.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cd.szxytkj.cn

JS:   arr.push(4);
来源：http://ph.jctech888.com.cn

TS:   arr.push(4);
来源：http://le.yuntaijiaju.cn

Java: list.add(4);
来源：http://fp.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://rn.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ke.huanxung.cn

C#:   list.Add(4);
来源：http://yc.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://nk.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://rc.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qz.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xd.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://fl.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ya.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rj.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ol.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://bv.huanxung.cn

[D04] 删除元素
来源：http://sq.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iq.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zp.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pd.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ve.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iw.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dr.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pf.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vt.chemitech.net.cn

[D05] 访问与修改元素
来源：http://tz.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://av.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xa.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ph.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://zw.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://xp.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://vt.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rj.shxzskj.cn

[D06] 数组长度
来源：http://wm.jianghongdianzi.cn

Py:   len(arr)
来源：http://pu.nszjky.cn

PHP:  count($arr);
来源：http://xr.huixiangedu.cn

JS:   arr.length
来源：http://zg.gzmigu.cn

TS:   arr.length
来源：http://os.hahajie.cn

Java: list.size();
来源：http://vw.shxzukj.cn

Go:   len(arr)
来源：http://wb.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://cs.jctech888.com.cn

C#:   list.Count;
来源：http://yz.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://yi.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ff.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ec.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://uz.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://by.nszjky.cn

Java: list.subList(1, 4);
来源：http://ux.huixiangedu.cn

Go:   arr[1:4]
来源：http://iz.szxytkj.cn

Ruby: arr[1, 3]
来源：http://gv.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://nz.lnxyls.cn

[D08] 合并两个数组
来源：http://kn.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://gr.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://pg.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ja.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ea.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://be.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://bq.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://xt.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://cp.szsharing.cn

[D09] 排序（升序）
来源：http://cx.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lp.yuexingan06.cn

PHP:  sort($arr);
来源：http://bs.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ol.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mb.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xu.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fu.lnxyls.cn

Ruby: arr.sort
来源：http://rn.nszjky.cn

C#:   list.Sort();
来源：http://ud.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mc.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xw.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jt.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xe.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xc.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tp.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lz.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dj.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uo.shxzskj.cn

[D11] 反转数组
来源：http://xe.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://np.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://ag.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://er.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://kc.shxzukj.cn

Java: Collections.reverse(list);
来源：http://yi.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://of.huanxung.cn

Ruby: arr.reverse
来源：http://ou.bookmarksfly.cn

C#:   list.Reverse();
来源：http://dg.gzmigu.cn

[D12] 查找元素下标
来源：http://at.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://rc.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pj.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ow.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xm.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://px.haigaiapp.cn

Ruby: arr.index(x)
来源：http://rs.nicolike.cn

C#:   list.IndexOf(x);
来源：http://wc.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://vp.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vc.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xq.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://xs.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://zl.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jg.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eo.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kk.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dv.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://gz.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ex.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tv.521024.cn

JS:   arr.map(x => x * 2)
来源：http://zg.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://hd.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iw.9csxet.cn

Go:   // 手写循环
来源：http://gp.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://in.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ux.muxihuayi.cn

[D15] 去重
来源：http://kq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mg.521024.cn

PHP:  array_unique($arr);
来源：http://tf.newstarts.cn

JS:   [...new Set(arr)]
来源：http://um.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ya.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wl.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ss.muxihuayi.cn

Ruby: arr.uniq
来源：http://xx.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://dy.shxzukj.cn

[D16] 求和与平均值
来源：http://jy.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gt.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zj.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zq.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pv.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oq.hnjuh.cn

Go:   // 手写循环累加
来源：http://te.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://on.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://kg.muxihuayi.cn

[D17] 最大值与最小值
来源：http://bf.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://qx.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://lo.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xw.szsharing.cn

TS:   Math.max(...arr);
来源：http://bf.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ku.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ys.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://xb.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://ou.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://dt.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ln.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://or.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://or.jianghongdianzi.cn

TS:   nested.flat();
来源：http://fv.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gv.chemitech.net.cn

Go:   // 手写双层循环
来源：http://xp.gzmigu.cn

Ruby: nested.flatten
来源：http://dk.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xb.panjiajie.cn

[D19] 按字段分组
来源：http://yh.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qf.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zh.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wm.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iw.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ys.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://tq.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sk.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vd.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://dd.nszjky.cn

Py:   Counter(arr)
来源：http://oc.521024.cn

PHP:  array_count_values($arr);
来源：http://kr.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tn.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://di.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ky.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://eg.shxzukj.cn

Ruby: arr.tally
来源：http://nu.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nd.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://fq.chemitech.net.cn

Py:   x in arr
来源：http://ie.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://dc.nszjky.cn

JS:   arr.includes(x)
来源：http://ml.hnjuh.cn

TS:   arr.includes(x)
来源：http://cm.huixinmuqiang.cn

Java: list.contains(x)
来源：http://od.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://or.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://gh.haigaiapp.cn

C#:   list.Contains(x)
来源：http://lk.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://sc.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xr.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ko.shtwfgs.cn

TS:   [...arr];
来源：http://sz.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://yo.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gy.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://no.huixiangedu.cn

C#:   new List<int>(list);
来源：http://rw.wgjwhj.cn

[D23] reduce 累积计算
来源：http://jb.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iz.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yj.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wt.hahajie.cn


<!-- 参考信息 -->