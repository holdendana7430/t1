代发 wailian999

[B13] 判断是否为数字
来源：http://ud.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://jg.lnxyls.cn

PHP:  is_numeric($x)
来源：http://py.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yd.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bb.lnxyls.cn

Java: x instanceof Number
来源：http://rp.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gp.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://tr.521024.cn

C#:   x is int or double or decimal
来源：http://ao.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://zm.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yz.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://el.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://jt.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ey.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://si.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vt.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ms.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kh.9csxet.cn

[B15] 布尔运算与取反
来源：http://ko.huixinmuqiang.cn

Py:   a and b or not c
来源：http://kz.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ku.jianghongdianzi.cn

JS:   a && b || !c
来源：http://zb.gzmigu.cn

TS:   a && b || !c
来源：http://ic.521024.cn

Java: a && b || !c
来源：http://ie.yuntaijiaju.cn

Go:   a && b || !c
来源：http://pz.szsharing.cn

Ruby: a && b || !c
来源：http://lj.shtwfgs.cn

C#:   a && b || !c
来源：http://wt.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mi.yuntaijiaju.cn

Py:   if not data: return
来源：http://hp.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://xi.asd995.cn

JS:   if (!data) return;
来源：http://um.panjiajie.cn

TS:   if (!data) return;
来源：http://fu.asd995.cn

Java: if (data == null) return;
来源：http://ez.asd995.cn

Go:   if data == nil { return }
来源：http://ve.shxzskj.cn

Ruby: return if data.nil?
来源：http://qj.chemitech.net.cn

C#:   if (data == null) return;
来源：http://on.shxzukj.cn

================================================================================
来源：http://bi.bookmarksfly.cn

C. 函数与作用域
来源：http://qh.shtwfgs.cn

================================================================================
来源：http://nc.yuexingan06.cn

[C01] 定义函数
来源：http://ir.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://hm.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nk.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://xl.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bg.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://es.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jm.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ls.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vs.jianghongdianzi.cn

[C02] 默认参数
来源：http://um.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://st.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ma.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://yq.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wd.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://za.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mg.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ja.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://es.hnjuh.cn

[C03] 可变参数
来源：http://qa.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://sg.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bg.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oo.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lm.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tg.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://up.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vw.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://yw.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://as.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bv.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qe.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ux.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ba.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://cj.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://jd.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://kp.szsharing.cn

[C05] 返回多个值
来源：http://hw.huixinmuqiang.cn

Py:   return a, b
来源：http://nb.colortex.cn

PHP:  return [$a, $b];
来源：http://ag.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aq.hahajie.cn

TS:   return { a, b };
来源：http://bi.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iy.bookmarksfly.cn

Go:   return a, b
来源：http://ur.chemitech.net.cn

Ruby: return a, b
来源：http://td.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pl.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ce.nicolike.cn

Py:   square = lambda x: x * x
来源：http://vm.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nz.lnxyls.cn

JS:   const square = x => x * x;
来源：http://iy.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ba.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fc.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qt.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://vk.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zj.asd995.cn

[C07] 把函数作为参数传入
来源：http://rl.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ck.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ju.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pz.newstarts.cn

TS:   arr.map(String)
来源：http://vi.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pb.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://co.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://kd.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vg.yuexingan06.cn

[C08] 闭包
来源：http://kt.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lk.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vu.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yf.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://se.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ql.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://py.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zl.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://az.yuntaijiaju.cn

[C09] 递归
来源：http://xp.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qd.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eh.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gz.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dv.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://il.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://br.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ra.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vt.bookmarksfly.cn

[C10] 变量作用域
来源：http://jb.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ea.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zn.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vb.lnxyls.cn

TS:   同 JS
来源：http://xa.panjiajie.cn

Java: 方法内为块级作用域
来源：http://uw.muxihuayi.cn

Go:   花括号块级作用域
来源：http://fa.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ec.chemitech.net.cn

C#:   块级作用域
来源：http://ce.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://nu.hnjuh.cn

Py:   from module import func
来源：http://jw.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://va.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://je.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qp.shxzskj.cn

Java: import java.util.List;
来源：http://yn.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pq.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://kn.szsharing.cn

C#:   using System.Text;
来源：http://ew.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://fa.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://dh.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://zp.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://lu.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://vb.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rt.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://hk.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://ib.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yo.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://cw.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mm.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vn.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uo.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vi.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xh.asd995.cn

Go:   func add(a, b int) int
来源：http://df.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kx.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wf.huixiangedu.cn

[C14] 泛型函数
来源：http://hs.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ab.wgjwhj.cn

PHP:  // 无泛型
来源：http://xp.panjiajie.cn

JS:   // 无泛型
来源：http://ko.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oq.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pu.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ci.szxytkj.cn

Ruby: # 无泛型
来源：http://pu.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lw.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://tm.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fa.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://ne.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tg.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yc.huanxung.cn

Java: // 无解构
来源：http://ab.huanxung.cn

Go:   // 无解构
来源：http://qz.gzmigu.cn

Ruby: a, b = pair
来源：http://gr.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ls.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://os.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hw.wgjwhj.cn

PHP:  // 无重载
来源：http://sw.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sq.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://gj.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sf.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://xz.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://bd.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ci.bookmarksfly.cn

================================================================================
来源：http://ze.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://tu.521024.cn

================================================================================
来源：http://se.hahajie.cn

[D01] 创建数组 / 列表
来源：http://uj.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://md.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nj.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wh.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ac.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rh.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://jf.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://py.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tn.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://mf.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jx.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zs.panjiajie.cn

JS:   arr.push(4);
来源：http://ze.huanxung.cn

TS:   arr.push(4);
来源：http://kj.bookmarksfly.cn

Java: list.add(4);
来源：http://wn.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://qa.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://cy.9csxet.cn

C#:   list.Add(4);
来源：http://vm.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://ne.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://fu.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fg.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xh.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://rm.gzmigu.cn

Java: list.add(0, 0);
来源：http://ir.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ej.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://na.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://xl.shtwfgs.cn

[D04] 删除元素
来源：http://tc.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ej.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://se.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vw.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://mm.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tu.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pm.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fw.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xs.521024.cn

[D05] 访问与修改元素
来源：http://mq.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ui.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jv.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wd.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://uu.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://cz.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://mx.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ve.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ul.yuntaijiaju.cn

[D06] 数组长度
来源：http://aw.yuntaijiaju.cn

Py:   len(arr)
来源：http://me.newstarts.cn

PHP:  count($arr);
来源：http://qs.muxihuayi.cn

JS:   arr.length
来源：http://wa.shtwfgs.cn

TS:   arr.length
来源：http://ru.newstarts.cn

Java: list.size();
来源：http://sm.huanxung.cn

Go:   len(arr)
来源：http://gv.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://st.bjjhwx.cn

C#:   list.Count;
来源：http://or.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://vn.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://et.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mt.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://md.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://fi.nicolike.cn

Java: list.subList(1, 4);
来源：http://hq.nszjky.cn

Go:   arr[1:4]
来源：http://zy.9csxet.cn

Ruby: arr[1, 3]
来源：http://ys.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://op.jctech888.com.cn

[D08] 合并两个数组
来源：http://uc.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://uq.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://un.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kj.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://mm.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://np.colortex.cn

Go:   append(a, b...)
来源：http://po.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://wr.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://lx.haigaiapp.cn

[D09] 排序（升序）
来源：http://zr.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://wc.muxihuayi.cn

PHP:  sort($arr);
来源：http://bk.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wz.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oy.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vk.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fe.bookmarksfly.cn

Ruby: arr.sort
来源：http://gq.huixiangedu.cn

C#:   list.Sort();
来源：http://ld.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ve.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kn.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gr.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sx.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nn.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ad.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aj.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yz.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gd.jianghongdianzi.cn

[D11] 反转数组
来源：http://ah.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cq.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://pn.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yj.szxytkj.cn

TS:   [...arr].reverse();
来源：http://zc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://qi.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://xx.gzmigu.cn

Ruby: arr.reverse
来源：http://ri.haigaiapp.cn

C#:   list.Reverse();
来源：http://pl.chemitech.net.cn

[D12] 查找元素下标
来源：http://ur.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://rh.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ov.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zf.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bl.asd995.cn

Go:   slices.Index(arr, x)
来源：http://xr.nicolike.cn

Ruby: arr.index(x)
来源：http://fj.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://fe.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://vl.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eh.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wl.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ww.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://rq.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nf.nszjky.cn


<!-- 参考信息 -->