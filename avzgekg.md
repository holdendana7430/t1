代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ae.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://jd.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ab.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ch.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xx.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qi.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ii.haigaiapp.cn

Py:   a and b or not c
来源：http://cn.huanxung.cn

PHP:  $a && $b || !$c
来源：http://gj.colortex.cn

JS:   a && b || !c
来源：http://fi.shxzskj.cn

TS:   a && b || !c
来源：http://of.jctech888.com.cn

Java: a && b || !c
来源：http://ui.shtwfgs.cn

Go:   a && b || !c
来源：http://ok.gzmigu.cn

Ruby: a && b || !c
来源：http://sb.wgjwhj.cn

C#:   a && b || !c
来源：http://sk.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mc.chemitech.net.cn

Py:   if not data: return
来源：http://mw.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://ac.chemitech.net.cn

JS:   if (!data) return;
来源：http://ux.muxihuayi.cn

TS:   if (!data) return;
来源：http://ra.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://xe.lnxyls.cn

Go:   if data == nil { return }
来源：http://zv.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ax.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ui.wgjwhj.cn

================================================================================
来源：http://lj.huixinmuqiang.cn

C. 函数与作用域
来源：http://ky.muxihuayi.cn

================================================================================
来源：http://rc.asd995.cn

[C01] 定义函数
来源：http://lm.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://vn.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nj.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://zz.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rp.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ok.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ct.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://eh.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kv.hahajie.cn

[C02] 默认参数
来源：http://ip.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://dp.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gk.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ke.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mj.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kv.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sb.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://tq.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://gu.colortex.cn

[C03] 可变参数
来源：http://bc.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://si.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://st.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vf.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yt.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://md.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yf.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ge.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jk.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://bb.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zw.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sk.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zi.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jy.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://tb.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://in.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://ni.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://ql.huanxung.cn

[C05] 返回多个值
来源：http://lb.nicolike.cn

Py:   return a, b
来源：http://qf.nszjky.cn

PHP:  return [$a, $b];
来源：http://jw.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fu.szsharing.cn

TS:   return { a, b };
来源：http://fy.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sj.wgjwhj.cn

Go:   return a, b
来源：http://qa.nszjky.cn

Ruby: return a, b
来源：http://bv.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://mw.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://rw.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://rx.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yd.panjiajie.cn

JS:   const square = x => x * x;
来源：http://dl.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://bl.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ow.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hd.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://kq.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://io.newstarts.cn

[C07] 把函数作为参数传入
来源：http://uq.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fx.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yh.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ke.asd995.cn

TS:   arr.map(String)
来源：http://jj.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://er.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ti.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://cd.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wu.szxytkj.cn

[C08] 闭包
来源：http://pt.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hq.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cy.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qc.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://np.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lr.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://il.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rt.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.asd995.cn

[C09] 递归
来源：http://ai.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qz.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xk.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ov.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://io.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nb.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nh.wgjwhj.cn

[C10] 变量作用域
来源：http://ff.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sj.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cd.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vd.muxihuayi.cn

TS:   同 JS
来源：http://jw.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://xc.chemitech.net.cn

Go:   花括号块级作用域
来源：http://lv.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tf.colortex.cn

C#:   块级作用域
来源：http://qa.shtwfgs.cn

[C11] 模块导入与导出
来源：http://hh.bookmarksfly.cn

Py:   from module import func
来源：http://io.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pg.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://po.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jc.hahajie.cn

Java: import java.util.List;
来源：http://qj.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jx.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://wp.lnxyls.cn

C#:   using System.Text;
来源：http://zv.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://il.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://lz.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ur.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://lu.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ms.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eh.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://jr.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://zj.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://og.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://dv.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eq.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://se.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yl.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bb.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://cg.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gq.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pl.shxzukj.cn

[C14] 泛型函数
来源：http://el.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aj.szsharing.cn

PHP:  // 无泛型
来源：http://er.lnxyls.cn

JS:   // 无泛型
来源：http://rx.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wz.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wd.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cf.nicolike.cn

Ruby: # 无泛型
来源：http://eo.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://df.hahajie.cn

[C15] 解构 / 展开参数
来源：http://py.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zi.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://tu.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hm.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xu.shxzukj.cn

Java: // 无解构
来源：http://cm.jctech888.com.cn

Go:   // 无解构
来源：http://ql.asd995.cn

Ruby: a, b = pair
来源：http://ht.asd995.cn

C#:   var (a, b) = pair;
来源：http://qj.asd995.cn

[C16] 函数 / 方法重载
来源：http://in.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rj.szxytkj.cn

PHP:  // 无重载
来源：http://lu.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://si.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://qr.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ke.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://mt.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://we.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vc.panjiajie.cn

================================================================================
来源：http://yn.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://iq.szxytkj.cn

================================================================================
来源：http://cg.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://rc.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oe.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vz.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://en.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xi.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pw.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://ot.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://go.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ih.colortex.cn

[D02] 追加元素到末尾
来源：http://no.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fs.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ny.shtwfgs.cn

JS:   arr.push(4);
来源：http://tv.lnxyls.cn

TS:   arr.push(4);
来源：http://sf.gzmigu.cn

Java: list.add(4);
来源：http://jg.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://ak.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://fu.wgjwhj.cn

C#:   list.Add(4);
来源：http://be.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://wu.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://he.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pe.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rf.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://es.muxihuayi.cn

Java: list.add(0, 0);
来源：http://cj.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wn.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oj.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://xn.newstarts.cn

[D04] 删除元素
来源：http://ro.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vn.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gw.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hq.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ak.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mp.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cj.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nw.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ld.huixiangedu.cn

[D05] 访问与修改元素
来源：http://sv.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bw.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nj.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ta.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://oq.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://cy.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://fp.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nn.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bl.shxzskj.cn

[D06] 数组长度
来源：http://bi.nszjky.cn

Py:   len(arr)
来源：http://ew.muxihuayi.cn

PHP:  count($arr);
来源：http://of.szxytkj.cn

JS:   arr.length
来源：http://yi.huixiangedu.cn

TS:   arr.length
来源：http://ev.huanxung.cn

Java: list.size();
来源：http://ba.newstarts.cn

Go:   len(arr)
来源：http://jk.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://fx.chemitech.net.cn

C#:   list.Count;
来源：http://tn.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://oc.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eh.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aj.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ec.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://jm.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://es.wgjwhj.cn

Go:   arr[1:4]
来源：http://yl.asd995.cn

Ruby: arr[1, 3]
来源：http://qh.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://zt.panjiajie.cn

[D08] 合并两个数组
来源：http://bu.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://vf.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://my.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://af.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ex.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iy.jctech888.com.cn

Go:   append(a, b...)
来源：http://eh.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://xz.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://of.huixiangedu.cn

[D09] 排序（升序）
来源：http://mc.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://nm.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://zy.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nv.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kp.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iu.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qx.panjiajie.cn

Ruby: arr.sort
来源：http://bp.panjiajie.cn

C#:   list.Sort();
来源：http://db.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://po.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kf.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gz.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bl.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uh.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mz.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fd.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dm.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wx.jctech888.com.cn

[D11] 反转数组
来源：http://ke.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rj.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://ho.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ub.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://dy.szsharing.cn

Java: Collections.reverse(list);
来源：http://eb.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://fc.yuexingan06.cn

Ruby: arr.reverse
来源：http://mh.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://nm.shtwfgs.cn

[D12] 查找元素下标
来源：http://ko.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://yo.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ua.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kv.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hi.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qm.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://ps.nicolike.cn

Ruby: arr.index(x)
来源：http://hu.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://pv.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ld.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mj.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nd.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://vs.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://et.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fu.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zq.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://um.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fq.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://nh.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ou.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://we.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://uy.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://no.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zi.shxzukj.cn

Go:   // 手写循环
来源：http://bd.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sj.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fw.huanxung.cn


<!-- 参考信息 -->