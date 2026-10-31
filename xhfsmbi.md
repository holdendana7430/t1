代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yk.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zc.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dv.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sd.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ea.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ar.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://pj.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://na.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vs.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ra.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hg.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ez.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://cd.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://hu.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://cm.shxzskj.cn

[C05] 返回多个值
来源：http://gg.shtwfgs.cn

Py:   return a, b
来源：http://gx.nszjky.cn

PHP:  return [$a, $b];
来源：http://np.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oc.shtwfgs.cn

TS:   return { a, b };
来源：http://lu.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yg.hahajie.cn

Go:   return a, b
来源：http://zz.chemitech.net.cn

Ruby: return a, b
来源：http://bl.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ji.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://hp.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://ro.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fr.nicolike.cn

JS:   const square = x => x * x;
来源：http://kc.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://co.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lv.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qf.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ad.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iz.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://ec.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gx.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://as.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wa.szxytkj.cn

TS:   arr.map(String)
来源：http://ed.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jm.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gf.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://nb.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ra.panjiajie.cn

[C08] 闭包
来源：http://mi.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qr.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uu.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fy.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vq.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dv.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qc.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yk.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zb.szsharing.cn

[C09] 递归
来源：http://gl.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vf.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ae.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ws.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://py.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hl.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://im.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gc.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gt.lnxyls.cn

[C10] 变量作用域
来源：http://wl.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bs.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ue.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lm.szsharing.cn

TS:   同 JS
来源：http://ng.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://cv.nszjky.cn

Go:   花括号块级作用域
来源：http://yf.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tr.shxzukj.cn

C#:   块级作用域
来源：http://tn.huixiangedu.cn

[C11] 模块导入与导出
来源：http://jc.jianghongdianzi.cn

Py:   from module import func
来源：http://ju.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uk.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hg.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ap.shtwfgs.cn

Java: import java.util.List;
来源：http://jd.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bg.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://vj.szxytkj.cn

C#:   using System.Text;
来源：http://xy.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://yi.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://sv.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://og.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://hu.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ui.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wy.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://rt.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://ur.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nj.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://cc.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eo.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gs.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zt.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ay.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lx.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ya.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bn.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xg.hnjuh.cn

[C14] 泛型函数
来源：http://dj.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tv.shxzukj.cn

PHP:  // 无泛型
来源：http://ud.panjiajie.cn

JS:   // 无泛型
来源：http://mc.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oe.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wx.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xt.asd995.cn

Ruby: # 无泛型
来源：http://hg.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ha.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://gt.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vg.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://wv.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iy.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ve.jctech888.com.cn

Java: // 无解构
来源：http://pe.panjiajie.cn

Go:   // 无解构
来源：http://ys.asd995.cn

Ruby: a, b = pair
来源：http://dd.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://vz.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://ih.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ge.shxzskj.cn

PHP:  // 无重载
来源：http://iz.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ta.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://ia.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fq.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://ld.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://kk.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yz.hnjuh.cn

================================================================================
来源：http://zw.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://si.newstarts.cn

================================================================================
来源：http://ih.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://sy.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ql.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://is.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kw.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hh.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cv.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://hp.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://nf.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kf.521024.cn

[D02] 追加元素到末尾
来源：http://uo.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://er.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xe.szsharing.cn

JS:   arr.push(4);
来源：http://lc.chemitech.net.cn

TS:   arr.push(4);
来源：http://bb.nicolike.cn

Java: list.add(4);
来源：http://ph.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://xm.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ug.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://ng.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://xc.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://fb.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oz.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uj.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://sm.chemitech.net.cn

Java: list.add(0, 0);
来源：http://of.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lg.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oq.521024.cn

C#:   list.Insert(0, 0);
来源：http://oy.hahajie.cn

[D04] 删除元素
来源：http://yo.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sv.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wd.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sn.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://eo.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rr.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dr.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ke.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mw.bjjhwx.cn

[D05] 访问与修改元素
来源：http://pf.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xu.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xt.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ti.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://bv.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://ma.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://kg.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ly.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ll.jianghongdianzi.cn

[D06] 数组长度
来源：http://cr.colortex.cn

Py:   len(arr)
来源：http://wp.shxzskj.cn

PHP:  count($arr);
来源：http://po.newstarts.cn

JS:   arr.length
来源：http://lf.shxzukj.cn

TS:   arr.length
来源：http://pt.szsharing.cn

Java: list.size();
来源：http://as.huixinmuqiang.cn

Go:   len(arr)
来源：http://wm.szsharing.cn

Ruby: arr.length; arr.size
来源：http://oo.asd995.cn

C#:   list.Count;
来源：http://ko.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://il.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://di.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hh.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://cb.colortex.cn

TS:   arr.slice(1, 4);
来源：http://oj.9csxet.cn

Java: list.subList(1, 4);
来源：http://qb.colortex.cn

Go:   arr[1:4]
来源：http://mz.gzmigu.cn

Ruby: arr[1, 3]
来源：http://rj.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://hk.haigaiapp.cn

[D08] 合并两个数组
来源：http://qz.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://nx.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://wi.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hy.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://by.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ms.jctech888.com.cn

Go:   append(a, b...)
来源：http://sq.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ah.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://em.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://yo.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://mn.yuexingan06.cn

PHP:  sort($arr);
来源：http://qp.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ok.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fn.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uc.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://se.shtwfgs.cn

Ruby: arr.sort
来源：http://xm.shtwfgs.cn

C#:   list.Sort();
来源：http://ma.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yn.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ln.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bb.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://id.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ku.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hj.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ja.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ao.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dd.haigaiapp.cn

[D11] 反转数组
来源：http://zd.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ya.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://gp.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ux.shxzukj.cn

TS:   [...arr].reverse();
来源：http://nl.shxzskj.cn

Java: Collections.reverse(list);
来源：http://qb.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://ui.szsharing.cn

Ruby: arr.reverse
来源：http://ng.hahajie.cn

C#:   list.Reverse();
来源：http://ti.newstarts.cn

[D12] 查找元素下标
来源：http://em.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://ci.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mo.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ww.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fw.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wv.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://bc.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://vx.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://dy.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://lo.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rk.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wx.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://un.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://od.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yy.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eh.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qi.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rl.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ii.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sl.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wm.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://gh.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://fs.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rm.huanxung.cn

Go:   // 手写循环
来源：http://hc.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ul.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tt.shtwfgs.cn

[D15] 去重
来源：http://oe.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ie.huanxung.cn

PHP:  array_unique($arr);
来源：http://ff.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://br.huanxung.cn

TS:   [...new Set(arr)]
来源：http://gj.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rl.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vl.yuexingan06.cn

Ruby: arr.uniq
来源：http://ar.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://zy.shxzukj.cn

[D16] 求和与平均值
来源：http://ol.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://in.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kq.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://je.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lr.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ld.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://if.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tw.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://hf.wgjwhj.cn

[D17] 最大值与最小值
来源：http://eo.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://uf.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://le.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://of.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://lw.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ow.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ds.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://jy.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://uz.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://jt.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://js.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://tp.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oy.colortex.cn

TS:   nested.flat();
来源：http://gg.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xs.szsharing.cn

Go:   // 手写双层循环
来源：http://bw.newstarts.cn

Ruby: nested.flatten
来源：http://sz.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kx.colortex.cn

[D19] 按字段分组
来源：http://qi.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://no.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gr.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nk.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jp.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cs.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://xw.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fl.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vf.asd995.cn

[D20] 统计每个元素出现次数
来源：http://np.panjiajie.cn

Py:   Counter(arr)
来源：http://gy.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://ig.yuntaijiaju.cn


<!-- 参考信息 -->