代发 wailian999

[C06] 匿名函数 / lambda
来源：http://mh.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://yl.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uv.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ev.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://zi.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zm.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ah.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://vo.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hf.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://uy.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zu.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qc.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tz.colortex.cn

TS:   arr.map(String)
来源：http://fo.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qg.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://px.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://ti.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sz.huixinmuqiang.cn

[C08] 闭包
来源：http://hh.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zm.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ax.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ro.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xz.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ny.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nm.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ig.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tz.shxzskj.cn

[C09] 递归
来源：http://oz.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dm.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qp.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mf.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ma.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kb.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mo.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nm.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://us.hnjuh.cn

[C10] 变量作用域
来源：http://hq.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ux.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pp.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cj.yuntaijiaju.cn

TS:   同 JS
来源：http://oj.panjiajie.cn

Java: 方法内为块级作用域
来源：http://uj.chemitech.net.cn

Go:   花括号块级作用域
来源：http://sz.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rx.jctech888.com.cn

C#:   块级作用域
来源：http://sx.yuexingan06.cn

[C11] 模块导入与导出
来源：http://lw.jctech888.com.cn

Py:   from module import func
来源：http://uv.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fr.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://li.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://me.yuntaijiaju.cn

Java: import java.util.List;
来源：http://qm.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://li.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://an.chemitech.net.cn

C#:   using System.Text;
来源：http://md.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://st.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://pv.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://pk.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://cj.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://nf.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ri.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://no.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://ii.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fp.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://qz.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wf.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wz.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ze.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://le.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jf.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ce.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cj.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wz.chemitech.net.cn

[C14] 泛型函数
来源：http://ly.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://re.huixiangedu.cn

PHP:  // 无泛型
来源：http://bb.szxytkj.cn

JS:   // 无泛型
来源：http://lx.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ap.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hf.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qq.chemitech.net.cn

Ruby: # 无泛型
来源：http://op.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yg.newstarts.cn

[C15] 解构 / 展开参数
来源：http://zt.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ln.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://um.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gd.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jz.yuntaijiaju.cn

Java: // 无解构
来源：http://rw.newstarts.cn

Go:   // 无解构
来源：http://yh.wgjwhj.cn

Ruby: a, b = pair
来源：http://hv.colortex.cn

C#:   var (a, b) = pair;
来源：http://lr.huanxung.cn

[C16] 函数 / 方法重载
来源：http://rz.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ye.shxzukj.cn

PHP:  // 无重载
来源：http://uq.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hy.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://hr.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yj.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ux.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://so.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iq.shxzskj.cn

================================================================================
来源：http://wk.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://ze.lnxyls.cn

================================================================================
来源：http://qa.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ui.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hy.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pw.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yp.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zr.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://su.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ef.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://pt.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gw.hahajie.cn

[D02] 追加元素到末尾
来源：http://hv.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dv.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fy.wgjwhj.cn

JS:   arr.push(4);
来源：http://st.bookmarksfly.cn

TS:   arr.push(4);
来源：http://gn.haigaiapp.cn

Java: list.add(4);
来源：http://oe.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://kb.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://bd.bjjhwx.cn

C#:   list.Add(4);
来源：http://cl.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://sp.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://tp.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jf.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ht.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://qe.bjjhwx.cn

Java: list.add(0, 0);
来源：http://gs.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jc.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://us.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://np.shxzukj.cn

[D04] 删除元素
来源：http://tc.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wc.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oz.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tj.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://mx.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ei.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qo.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://im.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wx.chemitech.net.cn

[D05] 访问与修改元素
来源：http://lt.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jy.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ey.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ks.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://ne.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://dh.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://bf.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iu.chemitech.net.cn

[D06] 数组长度
来源：http://zh.haigaiapp.cn

Py:   len(arr)
来源：http://uj.wgjwhj.cn

PHP:  count($arr);
来源：http://rk.huixiangedu.cn

JS:   arr.length
来源：http://bh.hahajie.cn

TS:   arr.length
来源：http://ts.szxytkj.cn

Java: list.size();
来源：http://yu.huixinmuqiang.cn

Go:   len(arr)
来源：http://bp.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://jh.9csxet.cn

C#:   list.Count;
来源：http://rl.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://di.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://an.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yi.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://ei.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://yw.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://fr.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://jt.szxytkj.cn

Ruby: arr[1, 3]
来源：http://cv.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://pd.haigaiapp.cn

[D08] 合并两个数组
来源：http://wl.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://wm.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://co.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gf.bjjhwx.cn

TS:   [...a, ...b];
来源：http://bo.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://no.bookmarksfly.cn

Go:   append(a, b...)
来源：http://wu.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://gm.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://hy.asd995.cn

[D09] 排序（升序）
来源：http://jl.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://zn.jctech888.com.cn

PHP:  sort($arr);
来源：http://wg.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gs.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fd.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oe.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mh.shxzskj.cn

Ruby: arr.sort
来源：http://mf.lnxyls.cn

C#:   list.Sort();
来源：http://xi.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yy.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fb.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pp.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cc.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vm.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://od.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://at.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ze.muxihuayi.cn

[D11] 反转数组
来源：http://sp.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ir.szsharing.cn

PHP:  array_reverse($arr);
来源：http://vh.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xr.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://oh.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://av.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://le.shtwfgs.cn

Ruby: arr.reverse
来源：http://bj.shxzskj.cn

C#:   list.Reverse();
来源：http://pb.panjiajie.cn

[D12] 查找元素下标
来源：http://fz.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://jr.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gi.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ff.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vx.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yo.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ze.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://be.huanxung.cn

C#:   list.IndexOf(x);
来源：http://lj.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ld.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jd.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oa.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://jq.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rj.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://it.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fa.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gf.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://qp.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kn.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://po.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ou.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://br.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lp.hahajie.cn

Go:   // 手写循环
来源：http://wk.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fl.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qs.panjiajie.cn

[D15] 去重
来源：http://lq.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ca.newstarts.cn

PHP:  array_unique($arr);
来源：http://aa.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://kj.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://wi.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gd.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zq.gzmigu.cn

Ruby: arr.uniq
来源：http://bn.asd995.cn

C#:   list.Distinct().ToList()
来源：http://wf.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://qt.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rq.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qt.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fe.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xg.nicolike.cn

Go:   // 手写循环累加
来源：http://zy.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://di.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://co.shxzskj.cn

[D17] 最大值与最小值
来源：http://lw.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://lp.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://gb.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cc.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://zv.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oo.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vj.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://hu.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://mc.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://zm.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jk.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://xx.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xt.hahajie.cn

TS:   nested.flat();
来源：http://mf.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gz.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://jd.colortex.cn

Ruby: nested.flatten
来源：http://sb.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hb.wgjwhj.cn

[D19] 按字段分组
来源：http://pn.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ag.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://te.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hd.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rv.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dj.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://gn.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tq.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://es.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://ol.shxzukj.cn

Py:   Counter(arr)
来源：http://ft.asd995.cn

PHP:  array_count_values($arr);
来源：http://pc.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xn.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zy.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fv.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://ew.newstarts.cn

Ruby: arr.tally
来源：http://bp.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nw.colortex.cn

[D21] 判断是否包含某元素
来源：http://iq.wgjwhj.cn

Py:   x in arr
来源：http://mj.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://gz.colortex.cn

JS:   arr.includes(x)
来源：http://zc.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ev.huanxung.cn

Java: list.contains(x)
来源：http://dz.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://zs.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://oo.colortex.cn

C#:   list.Contains(x)
来源：http://dx.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://ze.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oi.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ck.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hg.shxzukj.cn

TS:   [...arr];
来源：http://vr.nszjky.cn

Java: new ArrayList<>(list);
来源：http://wd.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xr.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://tg.chemitech.net.cn

C#:   new List<int>(list);
来源：http://mh.lnxyls.cn


<!-- 参考信息 -->