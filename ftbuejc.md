代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://og.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lo.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qu.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gy.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zl.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://wj.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://ha.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://zj.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ii.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ib.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://sh.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kw.lnxyls.cn

[B12] 跳出多层循环
来源：http://ye.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jm.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hh.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oz.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ci.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ry.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uo.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sy.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://up.9csxet.cn

[B13] 判断是否为数字
来源：http://oe.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://nl.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://qt.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hh.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://di.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ij.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fi.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://jr.szxytkj.cn

C#:   x is int or double or decimal
来源：http://as.hahajie.cn

[B14] 判断值是否在集合内
来源：http://oz.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vh.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kg.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://lh.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://go.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hy.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://th.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ht.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://od.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://pm.haigaiapp.cn

Py:   a and b or not c
来源：http://it.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://zv.521024.cn

JS:   a && b || !c
来源：http://zw.haigaiapp.cn

TS:   a && b || !c
来源：http://uq.bjjhwx.cn

Java: a && b || !c
来源：http://fe.huixiangedu.cn

Go:   a && b || !c
来源：http://eb.szxytkj.cn

Ruby: a && b || !c
来源：http://ng.bjjhwx.cn

C#:   a && b || !c
来源：http://zu.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ny.szsharing.cn

Py:   if not data: return
来源：http://mt.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://dn.hnjuh.cn

JS:   if (!data) return;
来源：http://iz.shxzukj.cn

TS:   if (!data) return;
来源：http://ko.9csxet.cn

Java: if (data == null) return;
来源：http://ke.nszjky.cn

Go:   if data == nil { return }
来源：http://al.asd995.cn

Ruby: return if data.nil?
来源：http://yj.gzmigu.cn

C#:   if (data == null) return;
来源：http://qs.lnxyls.cn

================================================================================
来源：http://kb.shxzukj.cn

C. 函数与作用域
来源：http://uh.nicolike.cn

================================================================================
来源：http://cq.hnjuh.cn

[C01] 定义函数
来源：http://wn.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://dl.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ny.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://kg.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rj.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kp.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oz.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://xq.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uu.haigaiapp.cn

[C02] 默认参数
来源：http://db.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://pt.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gu.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://hs.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hn.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://na.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qo.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://rl.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://wh.bjjhwx.cn

[C03] 可变参数
来源：http://su.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ie.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sz.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cl.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ym.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wo.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dy.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wl.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bz.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://bj.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uw.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ug.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zf.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bc.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://pa.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://vl.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://yw.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://tk.hahajie.cn

[C05] 返回多个值
来源：http://ae.bookmarksfly.cn

Py:   return a, b
来源：http://vu.newstarts.cn

PHP:  return [$a, $b];
来源：http://cb.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lr.lnxyls.cn

TS:   return { a, b };
来源：http://dv.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mj.szxytkj.cn

Go:   return a, b
来源：http://su.gzmigu.cn

Ruby: return a, b
来源：http://az.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://ad.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://il.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://oa.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lv.nicolike.cn

JS:   const square = x => x * x;
来源：http://rg.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ne.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sw.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yb.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://eu.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wb.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://qt.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hd.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zl.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gq.hnjuh.cn

TS:   arr.map(String)
来源：http://bm.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jd.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uf.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://fd.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rw.jianghongdianzi.cn

[C08] 闭包
来源：http://jr.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lq.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tj.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dn.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tw.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ez.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://be.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xg.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kg.huixinmuqiang.cn

[C09] 递归
来源：http://kr.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gz.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kl.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xf.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pl.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cx.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://se.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mp.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://te.yuntaijiaju.cn

[C10] 变量作用域
来源：http://kj.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ef.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cm.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vx.shxzukj.cn

TS:   同 JS
来源：http://xs.lnxyls.cn

Java: 方法内为块级作用域
来源：http://yi.yuexingan06.cn

Go:   花括号块级作用域
来源：http://cu.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pi.huanxung.cn

C#:   块级作用域
来源：http://fc.wgjwhj.cn

[C11] 模块导入与导出
来源：http://zy.yuexingan06.cn

Py:   from module import func
来源：http://ev.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tz.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ul.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zz.jctech888.com.cn

Java: import java.util.List;
来源：http://nd.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lb.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://wm.panjiajie.cn

C#:   using System.Text;
来源：http://th.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://wm.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ql.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://fi.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://jd.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://rq.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vo.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://tx.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://me.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vv.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://gk.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tb.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cd.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yb.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://se.nicolike.cn

Go:   func add(a, b int) int
来源：http://pg.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mg.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jc.521024.cn

[C14] 泛型函数
来源：http://ga.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hs.chemitech.net.cn

PHP:  // 无泛型
来源：http://vg.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ba.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fe.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fi.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jq.bjjhwx.cn

Ruby: # 无泛型
来源：http://fr.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nr.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://ag.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dx.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://kq.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jo.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qe.yuexingan06.cn

Java: // 无解构
来源：http://hn.9csxet.cn

Go:   // 无解构
来源：http://tg.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://wj.colortex.cn

C#:   var (a, b) = pair;
来源：http://dm.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://ls.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gk.huanxung.cn

PHP:  // 无重载
来源：http://fp.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uh.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://km.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://am.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://sp.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://fm.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sp.shxzskj.cn

================================================================================
来源：http://cv.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://vd.hahajie.cn

================================================================================
来源：http://ye.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://bp.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mr.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wk.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://st.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fg.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://px.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://wh.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://lp.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://av.hahajie.cn

[D02] 追加元素到末尾
来源：http://qs.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nw.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ol.gzmigu.cn

JS:   arr.push(4);
来源：http://mf.muxihuayi.cn

TS:   arr.push(4);
来源：http://rk.jianghongdianzi.cn

Java: list.add(4);
来源：http://th.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://lg.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://cg.hahajie.cn

C#:   list.Add(4);
来源：http://uw.521024.cn

[D03] 在指定位置插入元素
来源：http://jh.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://jk.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://db.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mr.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://zj.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://lz.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ki.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sp.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://hp.haigaiapp.cn

[D04] 删除元素
来源：http://ix.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gf.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wd.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vw.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://wp.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cr.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gb.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vx.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gc.9csxet.cn

[D05] 访问与修改元素
来源：http://ff.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ad.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yp.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vk.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://lo.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://yw.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://om.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cj.panjiajie.cn

[D06] 数组长度
来源：http://zu.shxzskj.cn

Py:   len(arr)
来源：http://as.yuntaijiaju.cn

PHP:  count($arr);
来源：http://by.jctech888.com.cn

JS:   arr.length
来源：http://fj.haigaiapp.cn

TS:   arr.length
来源：http://wu.521024.cn

Java: list.size();
来源：http://rf.yuntaijiaju.cn

Go:   len(arr)
来源：http://rf.huanxung.cn

Ruby: arr.length; arr.size
来源：http://zl.nszjky.cn

C#:   list.Count;
来源：http://in.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ma.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gc.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tz.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://qr.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://lu.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://iq.shxzukj.cn

Go:   arr[1:4]
来源：http://eb.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://da.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://mp.colortex.cn

[D08] 合并两个数组
来源：http://oh.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://lr.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://me.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qs.nszjky.cn

TS:   [...a, ...b];
来源：http://fa.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ea.panjiajie.cn

Go:   append(a, b...)
来源：http://tg.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://en.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://ml.huanxung.cn

[D09] 排序（升序）
来源：http://mf.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://fw.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://rg.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zn.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oz.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lh.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://as.panjiajie.cn

Ruby: arr.sort
来源：http://oq.panjiajie.cn

C#:   list.Sort();
来源：http://qt.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wz.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qq.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://on.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ew.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://th.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hn.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dy.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vw.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oo.yuexingan06.cn


<!-- 参考信息 -->