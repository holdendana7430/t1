代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://uo.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sb.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://mc.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yd.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://or.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ot.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gl.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://au.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://kf.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://ha.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://tf.muxihuayi.cn

[C05] 返回多个值
来源：http://pt.szxytkj.cn

Py:   return a, b
来源：http://we.shxzukj.cn

PHP:  return [$a, $b];
来源：http://mr.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://th.huixiangedu.cn

TS:   return { a, b };
来源：http://sr.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aj.gzmigu.cn

Go:   return a, b
来源：http://ae.521024.cn

Ruby: return a, b
来源：http://jl.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://qs.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://ku.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://pi.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pg.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://gk.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://jk.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ha.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fg.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://qv.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tk.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ja.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dx.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lz.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lp.521024.cn

TS:   arr.map(String)
来源：http://et.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mw.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ai.521024.cn

Ruby: arr.map(&:upcase)
来源：http://fo.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zy.nicolike.cn

[C08] 闭包
来源：http://tp.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pt.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cj.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ql.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dz.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qj.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xx.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qw.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sx.nicolike.cn

[C09] 递归
来源：http://fm.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ej.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jk.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://np.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://td.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wp.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eb.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qw.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hr.lnxyls.cn

[C10] 变量作用域
来源：http://fs.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bl.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rd.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tl.jianghongdianzi.cn

TS:   同 JS
来源：http://ld.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://eq.newstarts.cn

Go:   花括号块级作用域
来源：http://zm.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bw.shxzukj.cn

C#:   块级作用域
来源：http://id.nicolike.cn

[C11] 模块导入与导出
来源：http://bc.huixiangedu.cn

Py:   from module import func
来源：http://qu.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nv.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xt.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hj.asd995.cn

Java: import java.util.List;
来源：http://sy.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gw.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://tk.huixiangedu.cn

C#:   using System.Text;
来源：http://fo.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://bz.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://pu.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://bx.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://bv.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://wd.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cv.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://kf.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://he.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://du.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://vh.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qi.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xq.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jp.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://il.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xs.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://cj.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fn.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zv.bjjhwx.cn

[C14] 泛型函数
来源：http://zn.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bx.asd995.cn

PHP:  // 无泛型
来源：http://jg.9csxet.cn

JS:   // 无泛型
来源：http://kq.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ux.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jm.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rq.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://wt.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ym.colortex.cn

[C15] 解构 / 展开参数
来源：http://tr.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sy.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://sk.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vz.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://po.newstarts.cn

Java: // 无解构
来源：http://zt.bjjhwx.cn

Go:   // 无解构
来源：http://gu.bookmarksfly.cn

Ruby: a, b = pair
来源：http://ak.szsharing.cn

C#:   var (a, b) = pair;
来源：http://gg.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://yb.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mk.szsharing.cn

PHP:  // 无重载
来源：http://rb.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eo.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://lw.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://la.521024.cn

Go:   // 无重载：用不同函数名
来源：http://pz.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://hq.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cb.nicolike.cn

================================================================================
来源：http://vf.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://fk.yuexingan06.cn

================================================================================
来源：http://hr.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://wh.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nb.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vs.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ud.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://si.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wl.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://gu.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://cn.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qf.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ii.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sz.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yo.shxzukj.cn

JS:   arr.push(4);
来源：http://ol.haigaiapp.cn

TS:   arr.push(4);
来源：http://xa.shxzukj.cn

Java: list.add(4);
来源：http://ys.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://hm.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://io.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://io.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://qw.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://bq.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bc.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ba.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://bd.huixiangedu.cn

Java: list.add(0, 0);
来源：http://sp.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lm.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yr.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://zu.haigaiapp.cn

[D04] 删除元素
来源：http://ln.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yh.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ug.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vb.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://zg.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cr.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vo.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vy.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eb.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ez.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ld.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://il.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://kj.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://pu.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://ww.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vg.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sg.521024.cn

[D06] 数组长度
来源：http://fq.lnxyls.cn

Py:   len(arr)
来源：http://nz.haigaiapp.cn

PHP:  count($arr);
来源：http://sx.huixiangedu.cn

JS:   arr.length
来源：http://xu.jctech888.com.cn

TS:   arr.length
来源：http://cg.gzmigu.cn

Java: list.size();
来源：http://iz.yuntaijiaju.cn

Go:   len(arr)
来源：http://cz.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://bk.nicolike.cn

C#:   list.Count;
来源：http://gt.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://xi.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zf.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nf.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://gr.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://fq.gzmigu.cn

Java: list.subList(1, 4);
来源：http://uu.colortex.cn

Go:   arr[1:4]
来源：http://ja.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://eb.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://gp.bjjhwx.cn

[D08] 合并两个数组
来源：http://go.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://nz.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://cu.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xb.yuexingan06.cn

TS:   [...a, ...b];
来源：http://fl.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dg.haigaiapp.cn

Go:   append(a, b...)
来源：http://wx.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://od.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://nw.shxzskj.cn

[D09] 排序（升序）
来源：http://dv.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kr.nszjky.cn

PHP:  sort($arr);
来源：http://nm.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vd.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sp.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wp.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ug.hnjuh.cn

Ruby: arr.sort
来源：http://su.nicolike.cn

C#:   list.Sort();
来源：http://vz.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pg.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qn.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://am.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mh.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kk.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://di.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sl.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bt.colortex.cn

[D11] 反转数组
来源：http://zd.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oh.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://te.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fz.asd995.cn

TS:   [...arr].reverse();
来源：http://vl.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://cf.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://jh.huanxung.cn

Ruby: arr.reverse
来源：http://xn.nszjky.cn

C#:   list.Reverse();
来源：http://dz.haigaiapp.cn

[D12] 查找元素下标
来源：http://ea.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://gi.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pz.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://si.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ms.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ob.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://cg.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ao.hahajie.cn

C#:   list.IndexOf(x);
来源：http://mz.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://sd.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mj.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mz.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://xk.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://vp.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zk.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rt.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zv.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cf.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://jx.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ka.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yo.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://iw.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://zx.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dx.hahajie.cn

Go:   // 手写循环
来源：http://bq.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wq.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qu.bookmarksfly.cn

[D15] 去重
来源：http://nj.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xi.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://bf.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://bh.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ms.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jy.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gj.shxzukj.cn

Ruby: arr.uniq
来源：http://dy.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://an.colortex.cn

[D16] 求和与平均值
来源：http://zl.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xu.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vt.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qp.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hn.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xi.lnxyls.cn

Go:   // 手写循环累加
来源：http://gk.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dm.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://nn.asd995.cn

[D17] 最大值与最小值
来源：http://mq.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://lr.521024.cn

PHP:  max($arr);  min($arr);
来源：http://by.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iz.nszjky.cn

TS:   Math.max(...arr);
来源：http://fg.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wg.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://np.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://yl.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://ev.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://bg.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ii.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://yg.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vj.panjiajie.cn

TS:   nested.flat();
来源：http://lh.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yn.shtwfgs.cn

Go:   // 手写双层循环
来源：http://dq.huixiangedu.cn

Ruby: nested.flatten
来源：http://ib.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uq.panjiajie.cn

[D19] 按字段分组
来源：http://zf.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xv.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yr.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xk.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bi.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ls.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://ej.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bq.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mn.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://dh.colortex.cn

Py:   Counter(arr)
来源：http://uy.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://bb.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bx.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jx.newstarts.cn

Go:   // 手写 map[T]int
来源：http://as.haigaiapp.cn


<!-- 参考信息 -->