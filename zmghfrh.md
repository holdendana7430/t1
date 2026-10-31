代发 wailian999

Py:   if not data: return
来源：http://fk.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://gv.asd995.cn

JS:   if (!data) return;
来源：http://ld.521024.cn

TS:   if (!data) return;
来源：http://kv.newstarts.cn

Java: if (data == null) return;
来源：http://xt.haigaiapp.cn

Go:   if data == nil { return }
来源：http://bj.huixiangedu.cn

Ruby: return if data.nil?
来源：http://qk.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ur.nszjky.cn

================================================================================
来源：http://ck.521024.cn

C. 函数与作用域
来源：http://zr.gzmigu.cn

================================================================================
来源：http://zz.hnjuh.cn

[C01] 定义函数
来源：http://kw.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://qf.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://um.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://yw.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kt.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uy.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://py.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://vu.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://el.shxzukj.cn

[C02] 默认参数
来源：http://dm.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://cj.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ei.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://qe.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iv.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gi.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mw.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://yf.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://at.chemitech.net.cn

[C03] 可变参数
来源：http://pq.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://js.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://up.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://no.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ia.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lp.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ek.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ud.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wh.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://vs.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hc.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zv.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wx.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sc.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://rx.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://pk.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://fr.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://fe.bookmarksfly.cn

[C05] 返回多个值
来源：http://tj.9csxet.cn

Py:   return a, b
来源：http://uk.panjiajie.cn

PHP:  return [$a, $b];
来源：http://do.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ws.9csxet.cn

TS:   return { a, b };
来源：http://oc.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lr.shtwfgs.cn

Go:   return a, b
来源：http://qj.hnjuh.cn

Ruby: return a, b
来源：http://rv.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://sp.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://by.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://vb.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oc.521024.cn

JS:   const square = x => x * x;
来源：http://be.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ab.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://df.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wn.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://jj.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cg.9csxet.cn

[C07] 把函数作为参数传入
来源：http://rs.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vi.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://an.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mv.panjiajie.cn

TS:   arr.map(String)
来源：http://hf.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kh.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://te.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://op.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zp.jctech888.com.cn

[C08] 闭包
来源：http://jj.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xd.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qz.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qb.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ig.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pd.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cq.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://is.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dt.huanxung.cn

[C09] 递归
来源：http://uo.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qp.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://im.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zd.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pg.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vt.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vy.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iw.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zg.shxzukj.cn

[C10] 变量作用域
来源：http://rv.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wa.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://va.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pj.newstarts.cn

TS:   同 JS
来源：http://ft.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://ie.muxihuayi.cn

Go:   花括号块级作用域
来源：http://ck.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xb.szxytkj.cn

C#:   块级作用域
来源：http://ii.colortex.cn

[C11] 模块导入与导出
来源：http://jb.huanxung.cn

Py:   from module import func
来源：http://st.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uv.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vf.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oh.szxytkj.cn

Java: import java.util.List;
来源：http://xa.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hh.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://zz.nicolike.cn

C#:   using System.Text;
来源：http://gf.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://nm.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://xv.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://yc.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://ze.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://la.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mr.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://fy.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://ar.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xj.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://xr.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rt.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ox.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vo.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nu.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gj.521024.cn

Go:   func add(a, b int) int
来源：http://mj.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kh.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yu.asd995.cn

[C14] 泛型函数
来源：http://sz.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hy.yuexingan06.cn

PHP:  // 无泛型
来源：http://oi.haigaiapp.cn

JS:   // 无泛型
来源：http://md.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gf.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zw.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lg.yuexingan06.cn

Ruby: # 无泛型
来源：http://qk.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lw.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://ou.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mb.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://qn.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pz.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kz.nszjky.cn

Java: // 无解构
来源：http://tv.huixinmuqiang.cn

Go:   // 无解构
来源：http://ts.colortex.cn

Ruby: a, b = pair
来源：http://ah.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://xh.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ni.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ej.521024.cn

PHP:  // 无重载
来源：http://no.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pw.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://sm.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kj.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://tb.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://ot.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://io.panjiajie.cn

================================================================================
来源：http://yj.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://mg.9csxet.cn

================================================================================
来源：http://vp.hahajie.cn

[D01] 创建数组 / 列表
来源：http://dm.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dt.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vz.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ez.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mw.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xz.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://rq.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://dp.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lw.nszjky.cn

[D02] 追加元素到末尾
来源：http://sf.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zm.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hu.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://jz.newstarts.cn

TS:   arr.push(4);
来源：http://aw.asd995.cn

Java: list.add(4);
来源：http://yw.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://pz.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://jw.huanxung.cn

C#:   list.Add(4);
来源：http://sl.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://tx.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://nl.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hq.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ku.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://vv.chemitech.net.cn

Java: list.add(0, 0);
来源：http://rc.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xm.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ce.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://so.jctech888.com.cn

[D04] 删除元素
来源：http://vh.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://st.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lh.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xr.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://rf.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ia.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wx.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rg.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ql.nicolike.cn

[D05] 访问与修改元素
来源：http://bv.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nw.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bx.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pr.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://zn.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://kk.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://pd.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bl.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fu.bjjhwx.cn

[D06] 数组长度
来源：http://jz.nszjky.cn

Py:   len(arr)
来源：http://qs.hnjuh.cn

PHP:  count($arr);
来源：http://nm.asd995.cn

JS:   arr.length
来源：http://ir.nicolike.cn

TS:   arr.length
来源：http://ax.yuntaijiaju.cn

Java: list.size();
来源：http://rv.asd995.cn

Go:   len(arr)
来源：http://gd.huanxung.cn

Ruby: arr.length; arr.size
来源：http://gs.lnxyls.cn

C#:   list.Count;
来源：http://nj.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://ex.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oj.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://di.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://sf.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://uo.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://yt.chemitech.net.cn

Go:   arr[1:4]
来源：http://dg.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://wp.521024.cn

C#:   list.GetRange(1, 3);
来源：http://tt.jctech888.com.cn

[D08] 合并两个数组
来源：http://zw.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://wb.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://zy.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ch.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://bo.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://or.lnxyls.cn

Go:   append(a, b...)
来源：http://iu.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://rv.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ix.chemitech.net.cn

[D09] 排序（升序）
来源：http://cs.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://bu.colortex.cn

PHP:  sort($arr);
来源：http://yn.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fp.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rb.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mp.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yr.shtwfgs.cn

Ruby: arr.sort
来源：http://xn.hnjuh.cn

C#:   list.Sort();
来源：http://ox.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gf.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ih.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mq.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ao.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tm.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://be.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vm.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cb.huixinmuqiang.cn

[D11] 反转数组
来源：http://eo.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xu.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://wx.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rv.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://ss.lnxyls.cn

Java: Collections.reverse(list);
来源：http://cb.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://db.muxihuayi.cn

Ruby: arr.reverse
来源：http://ei.chemitech.net.cn

C#:   list.Reverse();
来源：http://hj.chemitech.net.cn

[D12] 查找元素下标
来源：http://ag.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ib.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ju.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gr.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oj.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vh.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://jt.nicolike.cn

Ruby: arr.index(x)
来源：http://rm.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://wa.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://vb.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://di.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://et.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://mr.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://fq.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fc.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://br.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pb.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wa.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://zi.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lu.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zm.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://he.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://tj.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ci.lnxyls.cn

Go:   // 手写循环
来源：http://ms.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://px.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cu.hahajie.cn

[D15] 去重
来源：http://bz.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ls.9csxet.cn

PHP:  array_unique($arr);
来源：http://jt.newstarts.cn

JS:   [...new Set(arr)]
来源：http://kl.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://jo.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yb.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gv.szxytkj.cn

Ruby: arr.uniq
来源：http://wn.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ae.szsharing.cn

[D16] 求和与平均值
来源：http://od.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://re.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bk.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fy.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://af.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gd.gzmigu.cn

Go:   // 手写循环累加
来源：http://ud.lnxyls.cn


<!-- 参考信息 -->