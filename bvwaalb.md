代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ai.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://gz.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qv.szsharing.cn

[B12] 跳出多层循环
来源：http://df.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lh.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fs.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sm.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mr.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hs.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jx.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rc.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xw.huanxung.cn

[B13] 判断是否为数字
来源：http://ag.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://aw.nicolike.cn

PHP:  is_numeric($x)
来源：http://qj.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pd.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jc.huixinmuqiang.cn

Java: x instanceof Number
来源：http://gl.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mb.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ej.shxzukj.cn

C#:   x is int or double or decimal
来源：http://sp.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://bu.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ev.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sw.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://jw.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://kg.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iq.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uu.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eg.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xt.panjiajie.cn

[B15] 布尔运算与取反
来源：http://fp.huanxung.cn

Py:   a and b or not c
来源：http://du.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://jc.szxytkj.cn

JS:   a && b || !c
来源：http://ov.wgjwhj.cn

TS:   a && b || !c
来源：http://fu.bookmarksfly.cn

Java: a && b || !c
来源：http://ps.9csxet.cn

Go:   a && b || !c
来源：http://it.jctech888.com.cn

Ruby: a && b || !c
来源：http://dg.521024.cn

C#:   a && b || !c
来源：http://cp.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vy.muxihuayi.cn

Py:   if not data: return
来源：http://ty.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://ru.haigaiapp.cn

JS:   if (!data) return;
来源：http://ck.muxihuayi.cn

TS:   if (!data) return;
来源：http://wt.newstarts.cn

Java: if (data == null) return;
来源：http://nw.huanxung.cn

Go:   if data == nil { return }
来源：http://ib.shxzukj.cn

Ruby: return if data.nil?
来源：http://mr.nicolike.cn

C#:   if (data == null) return;
来源：http://eg.nszjky.cn

================================================================================
来源：http://ay.bookmarksfly.cn

C. 函数与作用域
来源：http://lb.gzmigu.cn

================================================================================
来源：http://lm.lnxyls.cn

[C01] 定义函数
来源：http://ig.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://gt.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://no.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nf.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aw.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ei.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ni.panjiajie.cn

[C02] 默认参数
来源：http://az.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://bo.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jw.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ab.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://km.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cq.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kd.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://le.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://kr.newstarts.cn

[C03] 可变参数
来源：http://ja.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://jy.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wp.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wf.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tg.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jc.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rl.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rd.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zi.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://ka.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tc.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ez.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://du.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qf.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://ge.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://vy.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://ik.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://yr.huanxung.cn

[C05] 返回多个值
来源：http://pj.9csxet.cn

Py:   return a, b
来源：http://nt.colortex.cn

PHP:  return [$a, $b];
来源：http://tb.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pg.wgjwhj.cn

TS:   return { a, b };
来源：http://rx.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fi.bjjhwx.cn

Go:   return a, b
来源：http://ho.huanxung.cn

Ruby: return a, b
来源：http://vi.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://wl.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://yb.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://wq.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lm.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://py.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://ff.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cq.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bo.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://vo.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sf.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://da.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rd.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wm.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hj.wgjwhj.cn

TS:   arr.map(String)
来源：http://ih.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pg.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wt.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://pf.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iv.521024.cn

[C08] 闭包
来源：http://cz.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dt.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qy.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ia.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pl.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mh.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sq.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ad.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://go.bookmarksfly.cn

[C09] 递归
来源：http://nq.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gf.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uh.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tl.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uk.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lb.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fx.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zy.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oo.nicolike.cn

[C10] 变量作用域
来源：http://yq.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gk.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yk.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rw.asd995.cn

TS:   同 JS
来源：http://bm.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://tc.lnxyls.cn

Go:   花括号块级作用域
来源：http://hp.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ud.chemitech.net.cn

C#:   块级作用域
来源：http://se.shxzskj.cn

[C11] 模块导入与导出
来源：http://ww.lnxyls.cn

Py:   from module import func
来源：http://nr.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qj.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ym.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hm.huixiangedu.cn

Java: import java.util.List;
来源：http://xa.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jj.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://oh.chemitech.net.cn

C#:   using System.Text;
来源：http://re.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://dk.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://lh.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://ts.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://yk.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://pp.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ju.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xp.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://yf.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pu.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://ic.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ux.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bn.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xd.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://to.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tc.nicolike.cn

Go:   func add(a, b int) int
来源：http://ny.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ue.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pm.huanxung.cn

[C14] 泛型函数
来源：http://nr.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yz.9csxet.cn

PHP:  // 无泛型
来源：http://hb.hahajie.cn

JS:   // 无泛型
来源：http://rf.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://af.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rz.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mm.muxihuayi.cn

Ruby: # 无泛型
来源：http://eo.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vs.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://mm.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ge.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://uk.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pu.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sj.jctech888.com.cn

Java: // 无解构
来源：http://gt.szsharing.cn

Go:   // 无解构
来源：http://jh.9csxet.cn

Ruby: a, b = pair
来源：http://se.hahajie.cn

C#:   var (a, b) = pair;
来源：http://mz.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://mv.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eq.szsharing.cn

PHP:  // 无重载
来源：http://az.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wt.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://kg.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lh.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ie.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://xg.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qk.bookmarksfly.cn

================================================================================
来源：http://ja.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://qt.hahajie.cn

================================================================================
来源：http://ax.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ig.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yt.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tq.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uf.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fo.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ro.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://na.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://nq.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xp.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://et.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ym.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ax.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://fu.shtwfgs.cn

TS:   arr.push(4);
来源：http://np.wgjwhj.cn

Java: list.add(4);
来源：http://mb.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://rb.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.szsharing.cn

C#:   list.Add(4);
来源：http://gi.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://mr.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://qe.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vd.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xr.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://pf.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://sz.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wb.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nz.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://yg.gzmigu.cn

[D04] 删除元素
来源：http://qo.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sr.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wr.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qg.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://qr.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rx.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oz.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vi.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sm.huanxung.cn

[D05] 访问与修改元素
来源：http://ux.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sr.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cj.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ht.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://in.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://vt.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://th.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pr.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fb.huixinmuqiang.cn

[D06] 数组长度
来源：http://xh.huanxung.cn

Py:   len(arr)
来源：http://ik.chemitech.net.cn

PHP:  count($arr);
来源：http://ey.wgjwhj.cn

JS:   arr.length
来源：http://qv.shtwfgs.cn

TS:   arr.length
来源：http://kk.szsharing.cn

Java: list.size();
来源：http://gr.gzmigu.cn

Go:   len(arr)
来源：http://hy.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://hg.wgjwhj.cn

C#:   list.Count;
来源：http://oj.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://hy.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ug.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hw.asd995.cn

JS:   arr.slice(1, 4);
来源：http://nj.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://yo.hnjuh.cn

Java: list.subList(1, 4);
来源：http://oo.shxzskj.cn

Go:   arr[1:4]
来源：http://nz.521024.cn

Ruby: arr[1, 3]
来源：http://do.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://ga.huixiangedu.cn

[D08] 合并两个数组
来源：http://pk.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://mo.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://eg.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wp.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://wt.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nq.521024.cn

Go:   append(a, b...)
来源：http://hb.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://rs.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://gq.shxzukj.cn

[D09] 排序（升序）
来源：http://xb.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://jw.shxzskj.cn

PHP:  sort($arr);
来源：http://se.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ju.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://al.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tb.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eu.nicolike.cn

Ruby: arr.sort
来源：http://hc.bookmarksfly.cn

C#:   list.Sort();
来源：http://am.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lr.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hq.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://je.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://js.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rb.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qf.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tg.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gx.colortex.cn

[D11] 反转数组
来源：http://xx.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aa.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://gm.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bm.gzmigu.cn

TS:   [...arr].reverse();
来源：http://cs.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://zu.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://is.muxihuayi.cn

Ruby: arr.reverse
来源：http://mk.bjjhwx.cn

C#:   list.Reverse();
来源：http://yp.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://fk.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://lc.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://da.shtwfgs.cn


<!-- 参考信息 -->