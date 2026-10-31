代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://qc.huixiangedu.cn

[C03] 可变参数
来源：http://cu.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://fv.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iq.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zd.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kw.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://om.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vp.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qj.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vd.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://oa.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sq.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gz.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gc.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://im.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://jt.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://mg.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://tn.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ex.hahajie.cn

[C05] 返回多个值
来源：http://hy.asd995.cn

Py:   return a, b
来源：http://ow.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://pq.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wg.haigaiapp.cn

TS:   return { a, b };
来源：http://ps.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xb.muxihuayi.cn

Go:   return a, b
来源：http://zp.lnxyls.cn

Ruby: return a, b
来源：http://ps.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://kw.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://cd.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://bw.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zc.newstarts.cn

JS:   const square = x => x * x;
来源：http://ku.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://af.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pw.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fb.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://rz.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xo.nszjky.cn

[C07] 把函数作为参数传入
来源：http://tx.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wl.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ll.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yt.lnxyls.cn

TS:   arr.map(String)
来源：http://zp.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://do.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ea.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://bo.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fp.bookmarksfly.cn

[C08] 闭包
来源：http://ch.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wt.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ys.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ng.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dq.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://do.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ac.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sj.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wa.shxzskj.cn

[C09] 递归
来源：http://yt.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tm.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bx.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lf.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pi.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://im.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vr.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qa.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rk.jianghongdianzi.cn

[C10] 变量作用域
来源：http://tj.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fo.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vg.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ef.shxzskj.cn

TS:   同 JS
来源：http://tt.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://al.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://du.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gq.szxytkj.cn

C#:   块级作用域
来源：http://pz.colortex.cn

[C11] 模块导入与导出
来源：http://wz.szsharing.cn

Py:   from module import func
来源：http://za.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pa.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ge.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fp.gzmigu.cn

Java: import java.util.List;
来源：http://fw.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pu.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://zp.yuexingan06.cn

C#:   using System.Text;
来源：http://mm.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://pa.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://jr.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ix.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://hu.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gd.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://mv.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://nk.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lf.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://cx.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fl.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pr.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xl.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zz.szxytkj.cn

Go:   func add(a, b int) int
来源：http://kq.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vf.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lv.nicolike.cn

[C14] 泛型函数
来源：http://gl.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jr.hnjuh.cn

PHP:  // 无泛型
来源：http://cn.huanxung.cn

JS:   // 无泛型
来源：http://qc.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qk.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cz.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://el.huanxung.cn

Ruby: # 无泛型
来源：http://sd.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mu.colortex.cn

[C15] 解构 / 展开参数
来源：http://ze.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ru.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://vg.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ni.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tq.haigaiapp.cn

Java: // 无解构
来源：http://bj.bookmarksfly.cn

Go:   // 无解构
来源：http://bi.shtwfgs.cn

Ruby: a, b = pair
来源：http://re.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://si.nicolike.cn

[C16] 函数 / 方法重载
来源：http://kc.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dn.9csxet.cn

PHP:  // 无重载
来源：http://cg.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ar.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://wg.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gf.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://pf.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://zk.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://px.521024.cn

================================================================================
来源：http://uw.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://ee.hahajie.cn

================================================================================
来源：http://ui.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://yn.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rl.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://th.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zm.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hs.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zl.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://mj.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://gq.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rx.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://xe.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oq.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uq.haigaiapp.cn

JS:   arr.push(4);
来源：http://nb.gzmigu.cn

TS:   arr.push(4);
来源：http://rx.shxzskj.cn

Java: list.add(4);
来源：http://wu.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://fm.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://as.huixiangedu.cn

C#:   list.Add(4);
来源：http://gc.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://pc.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ta.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jx.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cg.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://lg.shxzukj.cn

Java: list.add(0, 0);
来源：http://mv.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lj.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://in.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://jl.newstarts.cn

[D04] 删除元素
来源：http://oc.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://om.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pn.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lw.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://gk.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dm.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gb.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ed.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nd.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://gy.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zb.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sz.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ef.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gr.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://ir.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://ub.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sg.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.jctech888.com.cn

[D06] 数组长度
来源：http://yj.hnjuh.cn

Py:   len(arr)
来源：http://dp.huixiangedu.cn

PHP:  count($arr);
来源：http://kw.huixinmuqiang.cn

JS:   arr.length
来源：http://zz.bookmarksfly.cn

TS:   arr.length
来源：http://gi.huanxung.cn

Java: list.size();
来源：http://js.colortex.cn

Go:   len(arr)
来源：http://ni.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ca.wgjwhj.cn

C#:   list.Count;
来源：http://nr.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://lf.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pv.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rx.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://ib.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://ri.colortex.cn

Java: list.subList(1, 4);
来源：http://xm.bookmarksfly.cn

Go:   arr[1:4]
来源：http://kw.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://uk.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://me.colortex.cn

[D08] 合并两个数组
来源：http://pv.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://nm.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://yu.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gp.szxytkj.cn

TS:   [...a, ...b];
来源：http://rl.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oq.huixiangedu.cn

Go:   append(a, b...)
来源：http://tb.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://em.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://uu.huanxung.cn

[D09] 排序（升序）
来源：http://jt.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://qc.bjjhwx.cn

PHP:  sort($arr);
来源：http://zb.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sd.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://um.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dh.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ex.lnxyls.cn

Ruby: arr.sort
来源：http://hz.shxzskj.cn

C#:   list.Sort();
来源：http://sn.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ry.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uh.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cx.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jz.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mw.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rt.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sr.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zb.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cn.szxytkj.cn

[D11] 反转数组
来源：http://bg.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ug.newstarts.cn

PHP:  array_reverse($arr);
来源：http://xo.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://di.lnxyls.cn

TS:   [...arr].reverse();
来源：http://vh.huanxung.cn

Java: Collections.reverse(list);
来源：http://gm.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://tq.huixiangedu.cn

Ruby: arr.reverse
来源：http://ff.haigaiapp.cn

C#:   list.Reverse();
来源：http://jr.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://kj.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://qn.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://is.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://od.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cg.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sd.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://pw.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://mt.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ne.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ah.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lf.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lt.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://kg.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://of.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xy.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sb.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lf.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vi.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://yp.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zm.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uq.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://ve.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://ta.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lg.haigaiapp.cn

Go:   // 手写循环
来源：http://tn.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://se.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vw.nszjky.cn

[D15] 去重
来源：http://se.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xs.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://vr.colortex.cn

JS:   [...new Set(arr)]
来源：http://cz.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://ye.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bf.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://up.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://tc.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://gn.bookmarksfly.cn

[D16] 求和与平均值
来源：http://my.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fo.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uy.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://va.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tb.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://uc.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://it.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://pk.521024.cn

[D17] 最大值与最小值
来源：http://cj.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://aw.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://hv.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qf.szxytkj.cn

TS:   Math.max(...arr);
来源：http://ty.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xd.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wf.asd995.cn

Ruby: arr.max;  arr.min
来源：http://cn.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://ay.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ix.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dm.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://fe.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bb.asd995.cn

TS:   nested.flat();
来源：http://cm.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oa.shtwfgs.cn

Go:   // 手写双层循环
来源：http://dt.nszjky.cn

Ruby: nested.flatten
来源：http://sd.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rx.nicolike.cn

[D19] 按字段分组
来源：http://ar.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qe.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fl.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fx.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://em.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://qe.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://es.jianghongdianzi.cn


<!-- 参考信息 -->