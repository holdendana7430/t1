代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qb.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zz.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xp.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tt.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ha.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lv.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://zt.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://kp.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://yk.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tp.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pc.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cz.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://al.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://kl.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dm.lnxyls.cn

[B12] 跳出多层循环
来源：http://yx.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tn.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ds.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kb.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://og.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kk.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gy.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dp.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xm.panjiajie.cn

[B13] 判断是否为数字
来源：http://tg.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://px.9csxet.cn

PHP:  is_numeric($x)
来源：http://ce.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.nszjky.cn

Java: x instanceof Number
来源：http://wg.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ln.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://zw.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://lz.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://bb.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://be.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zi.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ug.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://he.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sh.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wq.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vh.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hd.nicolike.cn

[B15] 布尔运算与取反
来源：http://vd.huixinmuqiang.cn

Py:   a and b or not c
来源：http://ji.szsharing.cn

PHP:  $a && $b || !$c
来源：http://vr.nszjky.cn

JS:   a && b || !c
来源：http://qr.wgjwhj.cn

TS:   a && b || !c
来源：http://pk.yuexingan06.cn

Java: a && b || !c
来源：http://el.colortex.cn

Go:   a && b || !c
来源：http://el.shxzukj.cn

Ruby: a && b || !c
来源：http://ad.szsharing.cn

C#:   a && b || !c
来源：http://iy.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iq.hahajie.cn

Py:   if not data: return
来源：http://nz.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://te.muxihuayi.cn

JS:   if (!data) return;
来源：http://ab.bookmarksfly.cn

TS:   if (!data) return;
来源：http://qs.szsharing.cn

Java: if (data == null) return;
来源：http://gl.hahajie.cn

Go:   if data == nil { return }
来源：http://ja.colortex.cn

Ruby: return if data.nil?
来源：http://dp.521024.cn

C#:   if (data == null) return;
来源：http://un.yuntaijiaju.cn

================================================================================
来源：http://me.huixiangedu.cn

C. 函数与作用域
来源：http://qj.shxzskj.cn

================================================================================
来源：http://oe.gzmigu.cn

[C01] 定义函数
来源：http://ge.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://qf.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://as.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://zo.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ed.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bk.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vo.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://td.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ir.jianghongdianzi.cn

[C02] 默认参数
来源：http://wc.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://eh.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fr.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://ry.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://en.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mb.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gs.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://vo.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://mn.wgjwhj.cn

[C03] 可变参数
来源：http://in.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://jr.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ez.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qp.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xo.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fa.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://es.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ao.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qh.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://md.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ux.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bb.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ua.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yh.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://pt.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://kp.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://px.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://mu.asd995.cn

[C05] 返回多个值
来源：http://pw.jianghongdianzi.cn

Py:   return a, b
来源：http://le.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://gx.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dv.szsharing.cn

TS:   return { a, b };
来源：http://jo.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://im.gzmigu.cn

Go:   return a, b
来源：http://gu.chemitech.net.cn

Ruby: return a, b
来源：http://rk.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://sq.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://my.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://wf.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bt.521024.cn

JS:   const square = x => x * x;
来源：http://hm.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ow.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://os.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fl.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://rf.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zj.nicolike.cn

[C07] 把函数作为参数传入
来源：http://id.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bt.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hd.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xe.newstarts.cn

TS:   arr.map(String)
来源：http://qj.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zv.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kq.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ad.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://on.panjiajie.cn

[C08] 闭包
来源：http://re.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ww.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://di.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wd.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yn.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mi.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dr.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ea.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ci.haigaiapp.cn

[C09] 递归
来源：http://iz.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gm.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jk.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lx.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iz.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mo.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mz.lnxyls.cn

[C10] 变量作用域
来源：http://sh.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bp.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pt.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ec.yuexingan06.cn

TS:   同 JS
来源：http://bv.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://sp.gzmigu.cn

Go:   花括号块级作用域
来源：http://wk.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bl.huixiangedu.cn

C#:   块级作用域
来源：http://go.shxzukj.cn

[C11] 模块导入与导出
来源：http://gp.jianghongdianzi.cn

Py:   from module import func
来源：http://ku.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jf.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://np.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fg.shtwfgs.cn

Java: import java.util.List;
来源：http://pt.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://in.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://mo.huixinmuqiang.cn

C#:   using System.Text;
来源：http://qh.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://sv.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://rr.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://ht.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ik.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://lr.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ev.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://gn.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://mv.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wj.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://xs.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ba.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xd.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bm.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tc.colortex.cn

Go:   func add(a, b int) int
来源：http://ff.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://po.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ph.yuntaijiaju.cn

[C14] 泛型函数
来源：http://jd.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yw.panjiajie.cn

PHP:  // 无泛型
来源：http://mq.shxzskj.cn

JS:   // 无泛型
来源：http://zk.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ny.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mm.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cg.newstarts.cn

Ruby: # 无泛型
来源：http://cb.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bb.szsharing.cn

[C15] 解构 / 展开参数
来源：http://vj.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zk.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://lw.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uy.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jx.yuexingan06.cn

Java: // 无解构
来源：http://pp.bookmarksfly.cn

Go:   // 无解构
来源：http://ql.huanxung.cn

Ruby: a, b = pair
来源：http://rc.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://dc.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://mg.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pk.huixiangedu.cn

PHP:  // 无重载
来源：http://do.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aq.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://co.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cq.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://es.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://vh.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bw.szsharing.cn

================================================================================
来源：http://xv.colortex.cn

D. 数组 / 列表 / 集合
来源：http://zm.huixinmuqiang.cn

================================================================================
来源：http://vk.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://pt.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ut.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vu.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tg.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zm.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://li.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://qg.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://yb.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qf.9csxet.cn

[D02] 追加元素到末尾
来源：http://kn.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vy.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yg.yuexingan06.cn

JS:   arr.push(4);
来源：http://il.hahajie.cn

TS:   arr.push(4);
来源：http://ts.9csxet.cn

Java: list.add(4);
来源：http://xz.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://kl.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://aw.yuexingan06.cn

C#:   list.Add(4);
来源：http://as.521024.cn

[D03] 在指定位置插入元素
来源：http://nr.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://zu.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uh.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mr.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://lf.shxzukj.cn

Java: list.add(0, 0);
来源：http://ru.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ya.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zj.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://tq.huanxung.cn

[D04] 删除元素
来源：http://sa.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jb.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qr.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uk.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://mq.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wi.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gj.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tc.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rp.jctech888.com.cn

[D05] 访问与修改元素
来源：http://sn.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ry.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tu.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fp.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ap.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://cf.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://as.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pe.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qy.panjiajie.cn

[D06] 数组长度
来源：http://qg.lnxyls.cn

Py:   len(arr)
来源：http://jq.huixinmuqiang.cn

PHP:  count($arr);
来源：http://fh.bookmarksfly.cn

JS:   arr.length
来源：http://xo.chemitech.net.cn

TS:   arr.length
来源：http://pq.newstarts.cn

Java: list.size();
来源：http://wf.chemitech.net.cn

Go:   len(arr)
来源：http://lp.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://jw.521024.cn

C#:   list.Count;
来源：http://yz.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://yz.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ga.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://px.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://os.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://rb.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://dn.jctech888.com.cn

Go:   arr[1:4]
来源：http://nf.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://nm.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://vo.nszjky.cn

[D08] 合并两个数组
来源：http://zs.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://wk.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://tq.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ku.huanxung.cn

TS:   [...a, ...b];
来源：http://mt.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ly.shxzukj.cn

Go:   append(a, b...)
来源：http://tq.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://ez.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://qt.521024.cn

[D09] 排序（升序）
来源：http://tj.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ds.521024.cn

PHP:  sort($arr);
来源：http://hi.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bt.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vo.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gs.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mo.huixinmuqiang.cn

Ruby: arr.sort
来源：http://gl.gzmigu.cn

C#:   list.Sort();
来源：http://ms.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hi.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ro.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gr.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jo.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mu.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zx.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ch.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hn.huanxung.cn


<!-- 参考信息 -->