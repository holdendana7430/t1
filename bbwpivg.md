代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://kl.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://vk.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ly.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zm.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oq.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vu.colortex.cn

[B15] 布尔运算与取反
来源：http://ak.yuexingan06.cn

Py:   a and b or not c
来源：http://yq.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://pv.jianghongdianzi.cn

JS:   a && b || !c
来源：http://cd.521024.cn

TS:   a && b || !c
来源：http://bs.huixiangedu.cn

Java: a && b || !c
来源：http://fm.bjjhwx.cn

Go:   a && b || !c
来源：http://uw.szxytkj.cn

Ruby: a && b || !c
来源：http://ib.gzmigu.cn

C#:   a && b || !c
来源：http://zz.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://du.hahajie.cn

Py:   if not data: return
来源：http://sw.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://em.bjjhwx.cn

JS:   if (!data) return;
来源：http://if.colortex.cn

TS:   if (!data) return;
来源：http://gs.nicolike.cn

Java: if (data == null) return;
来源：http://qt.gzmigu.cn

Go:   if data == nil { return }
来源：http://xw.hnjuh.cn

Ruby: return if data.nil?
来源：http://xn.shxzukj.cn

C#:   if (data == null) return;
来源：http://pl.nszjky.cn

================================================================================
来源：http://xk.yuntaijiaju.cn

C. 函数与作用域
来源：http://zg.huixinmuqiang.cn

================================================================================
来源：http://ec.huanxung.cn

[C01] 定义函数
来源：http://fh.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://my.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tv.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://qt.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ve.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://js.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fc.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://or.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fq.szsharing.cn

[C02] 默认参数
来源：http://wz.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://qs.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mp.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://oe.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ix.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sj.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fz.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://xw.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gt.haigaiapp.cn

[C03] 可变参数
来源：http://xw.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://hg.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://me.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tt.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rr.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://af.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vt.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kh.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://tm.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ap.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bc.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ax.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://se.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://fs.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://oc.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://qh.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://ah.bookmarksfly.cn

[C05] 返回多个值
来源：http://dt.jianghongdianzi.cn

Py:   return a, b
来源：http://vz.lnxyls.cn

PHP:  return [$a, $b];
来源：http://vy.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oz.jctech888.com.cn

TS:   return { a, b };
来源：http://za.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://no.huixiangedu.cn

Go:   return a, b
来源：http://lm.yuntaijiaju.cn

Ruby: return a, b
来源：http://ya.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ft.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://gp.nicolike.cn

Py:   square = lambda x: x * x
来源：http://xs.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xe.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://xj.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://oq.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hc.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kx.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://pi.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ww.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://uy.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uk.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yb.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ki.huixiangedu.cn

TS:   arr.map(String)
来源：http://qq.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://io.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ok.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://zy.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xf.yuntaijiaju.cn

[C08] 闭包
来源：http://jv.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yl.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rr.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lh.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gv.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://on.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jh.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xm.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mu.lnxyls.cn

[C09] 递归
来源：http://we.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sg.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iu.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sv.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lw.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lh.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qm.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dn.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://db.huixinmuqiang.cn

[C10] 变量作用域
来源：http://oq.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://if.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sv.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tu.huanxung.cn

TS:   同 JS
来源：http://ij.nszjky.cn

Java: 方法内为块级作用域
来源：http://ww.shxzukj.cn

Go:   花括号块级作用域
来源：http://dl.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vd.nicolike.cn

C#:   块级作用域
来源：http://sq.wgjwhj.cn

[C11] 模块导入与导出
来源：http://gy.muxihuayi.cn

Py:   from module import func
来源：http://xl.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iz.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sh.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lf.9csxet.cn

Java: import java.util.List;
来源：http://ku.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mb.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ao.asd995.cn

C#:   using System.Text;
来源：http://rr.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://hj.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://qs.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://td.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://mv.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://id.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hw.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://vs.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://kg.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wj.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ii.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pg.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://do.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://od.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yh.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gk.newstarts.cn

Go:   func add(a, b int) int
来源：http://sl.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pt.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://px.shxzskj.cn

[C14] 泛型函数
来源：http://wl.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zs.colortex.cn

PHP:  // 无泛型
来源：http://sw.bjjhwx.cn

JS:   // 无泛型
来源：http://um.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ml.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ll.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cx.huixiangedu.cn

Ruby: # 无泛型
来源：http://bi.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uw.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ui.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xj.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://op.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eo.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mf.shxzskj.cn

Java: // 无解构
来源：http://tw.yuntaijiaju.cn

Go:   // 无解构
来源：http://lp.hnjuh.cn

Ruby: a, b = pair
来源：http://ow.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://eb.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ca.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://el.szxytkj.cn

PHP:  // 无重载
来源：http://ej.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fh.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ku.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ps.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ki.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://lz.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zq.nszjky.cn

================================================================================
来源：http://wo.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://py.wgjwhj.cn

================================================================================
来源：http://ne.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://dm.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ge.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ht.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cw.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ym.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jf.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://rn.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://sj.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://be.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://kv.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xn.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://je.jctech888.com.cn

JS:   arr.push(4);
来源：http://xe.szxytkj.cn

TS:   arr.push(4);
来源：http://fl.haigaiapp.cn

Java: list.add(4);
来源：http://il.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://ss.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://bb.hahajie.cn

C#:   list.Add(4);
来源：http://jv.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://mv.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://ou.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pc.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jh.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://bw.szsharing.cn

Java: list.add(0, 0);
来源：http://ml.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vz.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://st.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ap.hahajie.cn

[D04] 删除元素
来源：http://qu.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sd.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://it.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ey.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ue.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sm.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rk.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sw.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ui.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://qn.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lc.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lc.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lu.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://rf.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ca.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ec.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hr.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mt.chemitech.net.cn

[D06] 数组长度
来源：http://yi.shxzskj.cn

Py:   len(arr)
来源：http://ra.nicolike.cn

PHP:  count($arr);
来源：http://tv.chemitech.net.cn

JS:   arr.length
来源：http://xl.panjiajie.cn

TS:   arr.length
来源：http://je.chemitech.net.cn

Java: list.size();
来源：http://wz.9csxet.cn

Go:   len(arr)
来源：http://ql.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://vz.9csxet.cn

C#:   list.Count;
来源：http://oh.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://xe.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ir.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mp.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://zl.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://qu.szxytkj.cn

Java: list.subList(1, 4);
来源：http://yq.9csxet.cn

Go:   arr[1:4]
来源：http://pr.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://cc.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://bs.521024.cn

[D08] 合并两个数组
来源：http://fz.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://tw.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://lr.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zc.wgjwhj.cn

TS:   [...a, ...b];
来源：http://hy.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://se.colortex.cn

Go:   append(a, b...)
来源：http://lz.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ep.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://zd.nicolike.cn

[D09] 排序（升序）
来源：http://gz.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://kx.bjjhwx.cn

PHP:  sort($arr);
来源：http://bi.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cr.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://is.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xt.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pp.lnxyls.cn

Ruby: arr.sort
来源：http://au.shtwfgs.cn

C#:   list.Sort();
来源：http://vw.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ap.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hp.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sx.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nu.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hs.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mq.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kj.lnxyls.cn

[D11] 反转数组
来源：http://tx.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hx.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://bs.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bd.asd995.cn

TS:   [...arr].reverse();
来源：http://pp.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ui.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://om.shxzskj.cn

Ruby: arr.reverse
来源：http://di.gzmigu.cn

C#:   list.Reverse();
来源：http://bx.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ox.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://fn.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mh.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vl.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yi.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zs.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://ft.panjiajie.cn

Ruby: arr.index(x)
来源：http://rb.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://qj.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://yy.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bb.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bz.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://dz.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://xg.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ua.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zh.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oo.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gt.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mz.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kz.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://zz.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://uh.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://et.haigaiapp.cn

Go:   // 手写循环
来源：http://cj.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://at.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mu.shxzskj.cn


<!-- 参考信息 -->