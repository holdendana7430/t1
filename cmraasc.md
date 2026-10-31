代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://iy.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kn.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yu.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://kd.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ew.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://pv.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ws.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://og.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jf.chemitech.net.cn

TS:   arr.map(String)
来源：http://ga.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gy.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://up.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://kw.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://np.muxihuayi.cn

[C08] 闭包
来源：http://nk.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rt.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fd.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fd.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fu.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qw.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://st.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ch.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iz.521024.cn

[C09] 递归
来源：http://ot.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ik.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wf.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gj.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vr.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bi.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ff.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lp.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kw.asd995.cn

[C10] 变量作用域
来源：http://cm.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fi.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iq.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nl.shxzskj.cn

TS:   同 JS
来源：http://wn.colortex.cn

Java: 方法内为块级作用域
来源：http://aa.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://ao.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zh.colortex.cn

C#:   块级作用域
来源：http://ve.jctech888.com.cn

[C11] 模块导入与导出
来源：http://nd.colortex.cn

Py:   from module import func
来源：http://ge.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rp.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rq.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xk.chemitech.net.cn

Java: import java.util.List;
来源：http://tn.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tj.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://hx.muxihuayi.cn

C#:   using System.Text;
来源：http://wd.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://uj.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://wm.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ll.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://kx.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ed.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://kl.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://ib.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bo.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://kl.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://by.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qv.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sa.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ds.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wc.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://ia.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kk.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vh.huixinmuqiang.cn

[C14] 泛型函数
来源：http://um.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bj.bjjhwx.cn

PHP:  // 无泛型
来源：http://ws.yuntaijiaju.cn

JS:   // 无泛型
来源：http://rr.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uk.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nu.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mt.szsharing.cn

Ruby: # 无泛型
来源：http://nm.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wb.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://dn.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tx.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://tc.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ta.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mc.hahajie.cn

Java: // 无解构
来源：http://ol.huanxung.cn

Go:   // 无解构
来源：http://sk.hahajie.cn

Ruby: a, b = pair
来源：http://vo.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://nc.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://kv.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://my.newstarts.cn

PHP:  // 无重载
来源：http://kd.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yd.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://sj.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wr.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://cc.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://wo.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mq.wgjwhj.cn

================================================================================
来源：http://xn.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://un.lnxyls.cn

================================================================================
来源：http://rx.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://fz.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://db.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tt.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ba.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ph.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fr.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://ek.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://rl.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pm.hnjuh.cn

[D02] 追加元素到末尾
来源：http://qe.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vn.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ot.colortex.cn

JS:   arr.push(4);
来源：http://ot.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://sn.szxytkj.cn

Java: list.add(4);
来源：http://gf.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://rr.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://gg.panjiajie.cn

C#:   list.Add(4);
来源：http://ye.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://gg.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://kf.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zz.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ma.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://xf.shxzskj.cn

Java: list.add(0, 0);
来源：http://kj.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mj.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uf.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://so.szsharing.cn

[D04] 删除元素
来源：http://df.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cg.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ue.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qc.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://eo.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fh.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aj.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oe.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ju.szxytkj.cn

[D05] 访问与修改元素
来源：http://ws.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wv.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wh.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tz.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://fy.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://tr.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ke.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wa.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fl.521024.cn

[D06] 数组长度
来源：http://ox.jctech888.com.cn

Py:   len(arr)
来源：http://za.nszjky.cn

PHP:  count($arr);
来源：http://kp.bjjhwx.cn

JS:   arr.length
来源：http://oy.huixiangedu.cn

TS:   arr.length
来源：http://ra.bookmarksfly.cn

Java: list.size();
来源：http://eh.colortex.cn

Go:   len(arr)
来源：http://la.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://fp.panjiajie.cn

C#:   list.Count;
来源：http://kv.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://fx.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://py.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gh.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://hs.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://xn.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://yr.bookmarksfly.cn

Go:   arr[1:4]
来源：http://sc.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://mf.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://hs.hahajie.cn

[D08] 合并两个数组
来源：http://mf.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://bn.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://yz.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ie.gzmigu.cn

TS:   [...a, ...b];
来源：http://cr.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yd.lnxyls.cn

Go:   append(a, b...)
来源：http://ye.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://mj.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://fj.haigaiapp.cn

[D09] 排序（升序）
来源：http://qp.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ze.nszjky.cn

PHP:  sort($arr);
来源：http://du.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qs.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cn.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iv.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mn.lnxyls.cn

Ruby: arr.sort
来源：http://kn.gzmigu.cn

C#:   list.Sort();
来源：http://pq.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ke.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://te.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://am.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://og.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ai.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zc.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ub.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://za.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://if.szsharing.cn

[D11] 反转数组
来源：http://vv.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gb.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://jr.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aa.shxzskj.cn

TS:   [...arr].reverse();
来源：http://wg.szsharing.cn

Java: Collections.reverse(list);
来源：http://vt.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://hk.521024.cn

Ruby: arr.reverse
来源：http://la.bookmarksfly.cn

C#:   list.Reverse();
来源：http://xn.9csxet.cn

[D12] 查找元素下标
来源：http://ap.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ag.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://va.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bk.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hg.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jd.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://xm.hahajie.cn

Ruby: arr.index(x)
来源：http://mt.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://dn.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://cp.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://im.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ub.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://yh.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://jx.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pg.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ae.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lw.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jb.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://tu.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gv.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wd.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://aq.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://vm.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sd.gzmigu.cn

Go:   // 手写循环
来源：http://fv.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://br.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aa.nicolike.cn

[D15] 去重
来源：http://qq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hi.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://vg.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://xj.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ae.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yd.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ej.shtwfgs.cn

Ruby: arr.uniq
来源：http://xc.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://ee.shxzskj.cn

[D16] 求和与平均值
来源：http://ud.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bx.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zd.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dj.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oo.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ni.huanxung.cn

Go:   // 手写循环累加
来源：http://jy.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kh.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://jr.szsharing.cn

[D17] 最大值与最小值
来源：http://rf.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://ul.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://au.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yy.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://os.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sg.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lt.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://va.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://tr.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://iu.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mb.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://vv.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ae.gzmigu.cn

TS:   nested.flat();
来源：http://ia.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wt.colortex.cn

Go:   // 手写双层循环
来源：http://lm.hnjuh.cn

Ruby: nested.flatten
来源：http://ed.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lc.yuexingan06.cn

[D19] 按字段分组
来源：http://ry.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bi.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sc.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wt.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oj.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://wq.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://se.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gm.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://bg.newstarts.cn

Py:   Counter(arr)
来源：http://lb.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://dv.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ld.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fl.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gr.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://dt.nszjky.cn

Ruby: arr.tally
来源：http://qv.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jo.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://ja.muxihuayi.cn

Py:   x in arr
来源：http://ix.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://yp.colortex.cn

JS:   arr.includes(x)
来源：http://wf.wgjwhj.cn

TS:   arr.includes(x)
来源：http://ew.muxihuayi.cn

Java: list.contains(x)
来源：http://lr.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://qw.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://zk.gzmigu.cn

C#:   list.Contains(x)
来源：http://ku.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://kp.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wi.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ho.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yw.jctech888.com.cn

TS:   [...arr];
来源：http://ts.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://qb.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rk.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://jh.szxytkj.cn

C#:   new List<int>(list);
来源：http://xj.haigaiapp.cn

[D23] reduce 累积计算
来源：http://ie.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://le.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sm.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sr.panjiajie.cn


<!-- 参考信息 -->