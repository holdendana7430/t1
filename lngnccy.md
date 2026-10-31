代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ls.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kn.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://sw.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://hm.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ga.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uf.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wd.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kk.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wo.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://xj.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rj.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://vh.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gh.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cb.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ky.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wa.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iz.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cn.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hw.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cn.521024.cn

[B13] 判断是否为数字
来源：http://to.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://te.shxzskj.cn

PHP:  is_numeric($x)
来源：http://lo.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://io.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zk.asd995.cn

Java: x instanceof Number
来源：http://ed.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lm.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://iy.shxzskj.cn

C#:   x is int or double or decimal
来源：http://bj.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ps.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rs.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://di.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ug.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://su.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kz.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cl.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tm.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ab.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://sk.shtwfgs.cn

Py:   a and b or not c
来源：http://bw.asd995.cn

PHP:  $a && $b || !$c
来源：http://zp.jianghongdianzi.cn

JS:   a && b || !c
来源：http://ir.huixinmuqiang.cn

TS:   a && b || !c
来源：http://uc.shxzskj.cn

Java: a && b || !c
来源：http://uj.nicolike.cn

Go:   a && b || !c
来源：http://qw.wgjwhj.cn

Ruby: a && b || !c
来源：http://ta.colortex.cn

C#:   a && b || !c
来源：http://vl.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://re.haigaiapp.cn

Py:   if not data: return
来源：http://of.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://bq.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://uo.521024.cn

TS:   if (!data) return;
来源：http://oy.yuexingan06.cn

Java: if (data == null) return;
来源：http://qx.jctech888.com.cn

Go:   if data == nil { return }
来源：http://fc.huixiangedu.cn

Ruby: return if data.nil?
来源：http://di.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://pp.newstarts.cn

================================================================================
来源：http://qg.huixinmuqiang.cn

C. 函数与作用域
来源：http://xr.jctech888.com.cn

================================================================================
来源：http://gm.asd995.cn

[C01] 定义函数
来源：http://ju.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://kn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ww.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://bb.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uc.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hb.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pm.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ee.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wj.yuexingan06.cn

[C02] 默认参数
来源：http://ib.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ph.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fs.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://is.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://em.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hg.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kt.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://rw.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://sr.yuexingan06.cn

[C03] 可变参数
来源：http://ox.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://gv.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ep.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qc.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ov.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vx.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rh.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gk.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bf.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://bl.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sd.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bg.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qd.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tg.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://hn.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://of.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://pi.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://sw.gzmigu.cn

[C05] 返回多个值
来源：http://iz.jctech888.com.cn

Py:   return a, b
来源：http://bi.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://sy.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.lnxyls.cn

TS:   return { a, b };
来源：http://rt.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yb.hnjuh.cn

Go:   return a, b
来源：http://py.muxihuayi.cn

Ruby: return a, b
来源：http://fg.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://uv.colortex.cn

[C06] 匿名函数 / lambda
来源：http://ze.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://dj.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cl.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://dh.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://lo.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rx.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bi.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://we.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wd.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://gp.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bn.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ig.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uo.shtwfgs.cn

TS:   arr.map(String)
来源：http://kv.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rp.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jh.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://mu.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wo.haigaiapp.cn

[C08] 闭包
来源：http://be.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://di.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wp.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oa.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vs.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pj.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rz.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aa.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cj.bookmarksfly.cn

[C09] 递归
来源：http://he.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://do.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ry.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lo.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ii.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gw.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cf.panjiajie.cn

[C10] 变量作用域
来源：http://cy.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tu.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zb.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vm.wgjwhj.cn

TS:   同 JS
来源：http://xy.nicolike.cn

Java: 方法内为块级作用域
来源：http://kv.asd995.cn

Go:   花括号块级作用域
来源：http://pe.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rr.521024.cn

C#:   块级作用域
来源：http://yy.newstarts.cn

[C11] 模块导入与导出
来源：http://bt.nszjky.cn

Py:   from module import func
来源：http://rf.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vu.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ph.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ny.huixinmuqiang.cn

Java: import java.util.List;
来源：http://se.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gy.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://sh.bjjhwx.cn

C#:   using System.Text;
来源：http://qt.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ou.asd995.cn

Py:   (lambda: print("run"))()
来源：http://mm.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://yo.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://de.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://ui.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ay.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://as.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://lz.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nh.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://bj.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rk.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jz.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sw.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ck.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vc.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ua.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mi.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hr.muxihuayi.cn

[C14] 泛型函数
来源：http://fb.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fa.colortex.cn

PHP:  // 无泛型
来源：http://vi.wgjwhj.cn

JS:   // 无泛型
来源：http://le.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eq.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cb.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qf.9csxet.cn

Ruby: # 无泛型
来源：http://ou.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vg.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://my.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dv.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://jv.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ea.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nr.9csxet.cn

Java: // 无解构
来源：http://eo.szsharing.cn

Go:   // 无解构
来源：http://ut.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://bj.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://cy.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://bv.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ex.huixinmuqiang.cn

PHP:  // 无重载
来源：http://az.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hc.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://mn.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hs.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://zn.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://hm.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yr.newstarts.cn

================================================================================
来源：http://ih.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://sv.9csxet.cn

================================================================================
来源：http://et.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://bj.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rz.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tf.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://il.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xg.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tq.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://ch.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://me.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hm.gzmigu.cn

[D02] 追加元素到末尾
来源：http://wa.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://um.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tv.newstarts.cn

JS:   arr.push(4);
来源：http://mg.szxytkj.cn

TS:   arr.push(4);
来源：http://hf.nicolike.cn

Java: list.add(4);
来源：http://wd.asd995.cn

Go:   arr = append(arr, 4)
来源：http://va.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://uc.szxytkj.cn

C#:   list.Add(4);
来源：http://zu.521024.cn

[D03] 在指定位置插入元素
来源：http://en.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://uv.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qw.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nl.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://py.newstarts.cn

Java: list.add(0, 0);
来源：http://cc.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fn.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ub.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://yw.jctech888.com.cn

[D04] 删除元素
来源：http://ak.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rr.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lj.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ye.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://wu.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dx.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://du.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hk.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://in.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://zf.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ak.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://co.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lm.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://fk.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://uc.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://ni.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qg.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ix.nicolike.cn

[D06] 数组长度
来源：http://sf.shtwfgs.cn

Py:   len(arr)
来源：http://hs.chemitech.net.cn

PHP:  count($arr);
来源：http://yr.hahajie.cn

JS:   arr.length
来源：http://go.asd995.cn

TS:   arr.length
来源：http://uo.jianghongdianzi.cn

Java: list.size();
来源：http://xz.chemitech.net.cn

Go:   len(arr)
来源：http://ac.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://hk.shxzukj.cn

C#:   list.Count;
来源：http://iu.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://uc.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hu.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ud.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ls.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://pg.nicolike.cn

Java: list.subList(1, 4);
来源：http://di.newstarts.cn

Go:   arr[1:4]
来源：http://nk.colortex.cn

Ruby: arr[1, 3]
来源：http://cr.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://ih.hnjuh.cn

[D08] 合并两个数组
来源：http://ho.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://vj.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://br.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jx.szxytkj.cn

TS:   [...a, ...b];
来源：http://oi.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qe.szxytkj.cn

Go:   append(a, b...)
来源：http://np.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://ak.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://xe.gzmigu.cn

[D09] 排序（升序）
来源：http://gy.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.szxytkj.cn

PHP:  sort($arr);
来源：http://gu.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://je.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yu.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kh.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.huixiangedu.cn

Ruby: arr.sort
来源：http://dv.szsharing.cn

C#:   list.Sort();
来源：http://zb.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zw.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qp.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ch.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rl.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bi.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rj.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dw.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uw.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uz.521024.cn

[D11] 反转数组
来源：http://nt.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vb.hahajie.cn

PHP:  array_reverse($arr);
来源：http://cx.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cv.jianghongdianzi.cn


<!-- 参考信息 -->