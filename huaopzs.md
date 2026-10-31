代发 wailian999

PHP:  range(0, 10, 2);
来源：http://nb.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iq.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eg.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ex.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vj.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://zr.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uf.colortex.cn

[B12] 跳出多层循环
来源：http://xa.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fc.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fn.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gv.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vs.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nr.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mz.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eo.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rt.muxihuayi.cn

[B13] 判断是否为数字
来源：http://bw.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://xf.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://vt.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yp.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.haigaiapp.cn

Java: x instanceof Number
来源：http://gj.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fv.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://fd.asd995.cn

C#:   x is int or double or decimal
来源：http://ea.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://tk.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jo.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qk.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://se.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://el.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ui.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://di.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cg.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jd.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://rv.szxytkj.cn

Py:   a and b or not c
来源：http://sx.asd995.cn

PHP:  $a && $b || !$c
来源：http://gu.shxzukj.cn

JS:   a && b || !c
来源：http://of.yuntaijiaju.cn

TS:   a && b || !c
来源：http://fl.shtwfgs.cn

Java: a && b || !c
来源：http://cl.szxytkj.cn

Go:   a && b || !c
来源：http://ll.colortex.cn

Ruby: a && b || !c
来源：http://ro.hahajie.cn

C#:   a && b || !c
来源：http://bi.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ta.jianghongdianzi.cn

Py:   if not data: return
来源：http://ac.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://pq.asd995.cn

JS:   if (!data) return;
来源：http://cx.asd995.cn

TS:   if (!data) return;
来源：http://yv.hahajie.cn

Java: if (data == null) return;
来源：http://rr.gzmigu.cn

Go:   if data == nil { return }
来源：http://ac.wgjwhj.cn

Ruby: return if data.nil?
来源：http://zh.hnjuh.cn

C#:   if (data == null) return;
来源：http://ov.jctech888.com.cn

================================================================================
来源：http://oo.szsharing.cn

C. 函数与作用域
来源：http://ii.huanxung.cn

================================================================================
来源：http://oe.shtwfgs.cn

[C01] 定义函数
来源：http://os.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://bt.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://qc.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://te.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pa.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nk.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://ga.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lv.9csxet.cn

[C02] 默认参数
来源：http://vw.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://zj.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yz.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://zq.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hw.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zk.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vi.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://su.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nr.shtwfgs.cn

[C03] 可变参数
来源：http://oo.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://tj.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ki.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mo.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xz.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ka.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uy.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yw.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://du.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://vs.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ek.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vg.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qb.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://zg.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://nr.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://vz.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ov.szxytkj.cn

[C05] 返回多个值
来源：http://xi.szsharing.cn

Py:   return a, b
来源：http://tb.nszjky.cn

PHP:  return [$a, $b];
来源：http://cs.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vs.szsharing.cn

TS:   return { a, b };
来源：http://pc.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kj.haigaiapp.cn

Go:   return a, b
来源：http://ds.shxzukj.cn

Ruby: return a, b
来源：http://zi.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://kp.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://wr.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ar.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fr.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://cx.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://lq.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wh.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vo.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://wh.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://at.szsharing.cn

[C07] 把函数作为参数传入
来源：http://sy.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mj.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://su.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sp.muxihuayi.cn

TS:   arr.map(String)
来源：http://gp.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xv.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nl.521024.cn

Ruby: arr.map(&:upcase)
来源：http://dg.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cg.huixinmuqiang.cn

[C08] 闭包
来源：http://rx.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uo.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ep.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mw.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://li.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://va.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xp.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fs.lnxyls.cn

[C09] 递归
来源：http://fm.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ul.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ik.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bi.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lv.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ow.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yv.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iu.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jm.szsharing.cn

[C10] 变量作用域
来源：http://lr.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tf.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ol.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zd.shtwfgs.cn

TS:   同 JS
来源：http://ge.9csxet.cn

Java: 方法内为块级作用域
来源：http://ze.colortex.cn

Go:   花括号块级作用域
来源：http://cd.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wh.huanxung.cn

C#:   块级作用域
来源：http://tb.szsharing.cn

[C11] 模块导入与导出
来源：http://fz.bookmarksfly.cn

Py:   from module import func
来源：http://pf.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bh.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://za.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yw.9csxet.cn

Java: import java.util.List;
来源：http://vl.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mv.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ca.asd995.cn

C#:   using System.Text;
来源：http://gq.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://tq.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://cb.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://ug.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://jd.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://pd.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vn.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://fz.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://su.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wb.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://px.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pc.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nx.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iq.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ho.gzmigu.cn

Go:   func add(a, b int) int
来源：http://pl.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ps.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mc.lnxyls.cn

[C14] 泛型函数
来源：http://kc.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iw.521024.cn

PHP:  // 无泛型
来源：http://by.wgjwhj.cn

JS:   // 无泛型
来源：http://wt.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gv.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mw.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wv.asd995.cn

Ruby: # 无泛型
来源：http://mu.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jh.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://rr.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ys.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://cb.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zj.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nf.asd995.cn

Java: // 无解构
来源：http://jf.nszjky.cn

Go:   // 无解构
来源：http://lr.shxzskj.cn

Ruby: a, b = pair
来源：http://aq.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://wd.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ql.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ah.nicolike.cn

PHP:  // 无重载
来源：http://mu.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xs.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://gi.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xz.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://zy.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://bo.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cv.asd995.cn

================================================================================
来源：http://oa.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://cf.shxzukj.cn

================================================================================
来源：http://jw.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://mz.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bz.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rz.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ak.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dc.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zn.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://ad.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://jp.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sq.9csxet.cn

[D02] 追加元素到末尾
来源：http://wi.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zx.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dc.huanxung.cn

JS:   arr.push(4);
来源：http://nf.shxzukj.cn

TS:   arr.push(4);
来源：http://um.muxihuayi.cn

Java: list.add(4);
来源：http://pm.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://sq.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://gi.asd995.cn

C#:   list.Add(4);
来源：http://ku.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://wx.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://bf.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lq.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ui.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://an.colortex.cn

Java: list.add(0, 0);
来源：http://lx.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hq.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://km.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://kh.bookmarksfly.cn

[D04] 删除元素
来源：http://ox.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lz.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sj.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fi.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://xv.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ns.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://em.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yy.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qh.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ui.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mn.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cy.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jw.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://nl.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://sf.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://vg.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xd.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sp.hnjuh.cn

[D06] 数组长度
来源：http://fo.panjiajie.cn

Py:   len(arr)
来源：http://yl.nszjky.cn

PHP:  count($arr);
来源：http://pe.colortex.cn

JS:   arr.length
来源：http://tp.szxytkj.cn

TS:   arr.length
来源：http://wa.jctech888.com.cn

Java: list.size();
来源：http://nt.hnjuh.cn

Go:   len(arr)
来源：http://mh.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ue.newstarts.cn

C#:   list.Count;
来源：http://qe.huanxung.cn

[D07] 切片 / 取子数组
来源：http://xo.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mx.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ey.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ud.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://kg.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://la.bookmarksfly.cn

Go:   arr[1:4]
来源：http://hy.colortex.cn

Ruby: arr[1, 3]
来源：http://le.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ol.yuexingan06.cn

[D08] 合并两个数组
来源：http://vm.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://we.asd995.cn

PHP:  array_merge($a, $b);
来源：http://fj.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oo.nszjky.cn

TS:   [...a, ...b];
来源：http://tt.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qi.wgjwhj.cn

Go:   append(a, b...)
来源：http://ao.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://au.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://sj.521024.cn

[D09] 排序（升序）
来源：http://yg.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://pa.bjjhwx.cn

PHP:  sort($arr);
来源：http://rg.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xd.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ra.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://by.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jh.szxytkj.cn

Ruby: arr.sort
来源：http://ck.szxytkj.cn

C#:   list.Sort();
来源：http://sm.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bb.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ik.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yz.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cg.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://df.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ua.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kr.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fw.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cq.shxzukj.cn

[D11] 反转数组
来源：http://ne.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qs.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://id.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qk.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://lo.newstarts.cn

Java: Collections.reverse(list);
来源：http://am.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://jj.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ek.huanxung.cn


<!-- 参考信息 -->