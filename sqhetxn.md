代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://vk.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wg.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oh.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qv.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wy.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uv.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kp.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dd.nicolike.cn

[B13] 判断是否为数字
来源：http://yr.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://kh.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://sv.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oh.hnjuh.cn

Java: x instanceof Number
来源：http://xa.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ca.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://kv.colortex.cn

C#:   x is int or double or decimal
来源：http://ov.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ew.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ab.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gj.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://hw.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ff.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vh.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vu.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wn.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lq.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ym.huixiangedu.cn

Py:   a and b or not c
来源：http://rb.szsharing.cn

PHP:  $a && $b || !$c
来源：http://sg.jctech888.com.cn

JS:   a && b || !c
来源：http://cm.shxzskj.cn

TS:   a && b || !c
来源：http://oe.gzmigu.cn

Java: a && b || !c
来源：http://os.shxzskj.cn

Go:   a && b || !c
来源：http://oj.bjjhwx.cn

Ruby: a && b || !c
来源：http://iy.panjiajie.cn

C#:   a && b || !c
来源：http://le.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ca.huixinmuqiang.cn

Py:   if not data: return
来源：http://gd.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://xw.shtwfgs.cn

JS:   if (!data) return;
来源：http://bg.chemitech.net.cn

TS:   if (!data) return;
来源：http://kc.nicolike.cn

Java: if (data == null) return;
来源：http://an.lnxyls.cn

Go:   if data == nil { return }
来源：http://ht.521024.cn

Ruby: return if data.nil?
来源：http://dw.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://vl.shtwfgs.cn

================================================================================
来源：http://yd.jctech888.com.cn

C. 函数与作用域
来源：http://ug.huanxung.cn

================================================================================
来源：http://sn.9csxet.cn

[C01] 定义函数
来源：http://fq.521024.cn

Py:   def add(a, b): return a + b
来源：http://hd.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gm.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://bp.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kg.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://by.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nq.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://mj.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yj.huanxung.cn

[C02] 默认参数
来源：http://hb.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://pc.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zq.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://kk.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ka.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ba.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ad.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://bh.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ph.hahajie.cn

[C03] 可变参数
来源：http://ko.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://ju.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rc.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://th.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ja.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://im.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://df.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yf.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://gb.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tp.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oo.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://er.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xl.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ek.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://jc.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://ko.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://yw.panjiajie.cn

[C05] 返回多个值
来源：http://pn.huanxung.cn

Py:   return a, b
来源：http://zr.colortex.cn

PHP:  return [$a, $b];
来源：http://ay.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vr.huixiangedu.cn

TS:   return { a, b };
来源：http://an.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ip.nszjky.cn

Go:   return a, b
来源：http://tm.huanxung.cn

Ruby: return a, b
来源：http://ql.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://hi.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://zn.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://aq.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jl.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://na.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://yc.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lb.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://we.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://ra.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fh.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://aw.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wg.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zg.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.szxytkj.cn

TS:   arr.map(String)
来源：http://ax.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uo.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iu.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://nr.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oq.shxzukj.cn

[C08] 闭包
来源：http://bp.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xe.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zp.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oe.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cs.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yz.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wq.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wj.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fx.nicolike.cn

[C09] 递归
来源：http://fv.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wy.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xg.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://be.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lq.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jy.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wp.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://of.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://er.nszjky.cn

[C10] 变量作用域
来源：http://fi.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ph.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wl.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iq.9csxet.cn

TS:   同 JS
来源：http://qg.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://hd.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://gn.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zq.jianghongdianzi.cn

C#:   块级作用域
来源：http://te.hahajie.cn

[C11] 模块导入与导出
来源：http://gg.bjjhwx.cn

Py:   from module import func
来源：http://ip.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ot.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://du.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qj.huixinmuqiang.cn

Java: import java.util.List;
来源：http://au.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ml.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://nv.asd995.cn

C#:   using System.Text;
来源：http://zp.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://vs.colortex.cn

Py:   (lambda: print("run"))()
来源：http://rz.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://fw.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://gb.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ji.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://el.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ff.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://vf.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rk.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://ua.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pt.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cz.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nk.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nn.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://wm.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oc.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ev.huanxung.cn

[C14] 泛型函数
来源：http://wm.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://do.nicolike.cn

PHP:  // 无泛型
来源：http://vh.shxzukj.cn

JS:   // 无泛型
来源：http://fo.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pg.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fg.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ai.szxytkj.cn

Ruby: # 无泛型
来源：http://uz.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ab.nszjky.cn

[C15] 解构 / 展开参数
来源：http://km.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tb.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://la.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uk.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://va.yuntaijiaju.cn

Java: // 无解构
来源：http://an.gzmigu.cn

Go:   // 无解构
来源：http://xr.shxzskj.cn

Ruby: a, b = pair
来源：http://hb.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://yf.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://sn.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jc.jctech888.com.cn

PHP:  // 无重载
来源：http://hp.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wq.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://ut.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wk.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://pr.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://yt.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iw.yuexingan06.cn

================================================================================
来源：http://yc.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://uy.lnxyls.cn

================================================================================
来源：http://zb.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://zc.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bu.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tm.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cn.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ut.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://as.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://xf.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://yu.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://du.nszjky.cn

[D02] 追加元素到末尾
来源：http://nb.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uv.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tq.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://ql.colortex.cn

TS:   arr.push(4);
来源：http://uf.nszjky.cn

Java: list.add(4);
来源：http://gd.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://jy.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://sh.asd995.cn

C#:   list.Add(4);
来源：http://ea.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://kr.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://kl.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ns.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mx.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://gq.szxytkj.cn

Java: list.add(0, 0);
来源：http://fm.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mr.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xy.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://zb.muxihuayi.cn

[D04] 删除元素
来源：http://pa.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vt.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ap.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yc.521024.cn

TS:   arr.splice(0, 1);
来源：http://gz.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mt.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xj.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ds.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ag.muxihuayi.cn

[D05] 访问与修改元素
来源：http://wj.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tn.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uh.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://at.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://pn.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://ks.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ja.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://if.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nw.lnxyls.cn

[D06] 数组长度
来源：http://ym.9csxet.cn

Py:   len(arr)
来源：http://di.9csxet.cn

PHP:  count($arr);
来源：http://go.chemitech.net.cn

JS:   arr.length
来源：http://ro.hnjuh.cn

TS:   arr.length
来源：http://my.bjjhwx.cn

Java: list.size();
来源：http://xm.newstarts.cn

Go:   len(arr)
来源：http://zq.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://oq.shxzskj.cn

C#:   list.Count;
来源：http://ap.newstarts.cn

[D07] 切片 / 取子数组
来源：http://yo.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hc.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kz.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://bu.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://ku.521024.cn

Java: list.subList(1, 4);
来源：http://sf.lnxyls.cn

Go:   arr[1:4]
来源：http://ha.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://sj.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://xn.shtwfgs.cn

[D08] 合并两个数组
来源：http://pn.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://vy.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://cw.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aq.hahajie.cn

TS:   [...a, ...b];
来源：http://ju.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cu.colortex.cn

Go:   append(a, b...)
来源：http://sh.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://ex.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://xx.asd995.cn

[D09] 排序（升序）
来源：http://uq.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://hi.asd995.cn

PHP:  sort($arr);
来源：http://ns.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ui.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iv.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dv.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sd.lnxyls.cn

Ruby: arr.sort
来源：http://yf.jianghongdianzi.cn

C#:   list.Sort();
来源：http://sx.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ac.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ou.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vg.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xu.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oz.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mr.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jn.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tx.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jj.9csxet.cn

[D11] 反转数组
来源：http://uz.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://np.nicolike.cn

PHP:  array_reverse($arr);
来源：http://zt.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bl.lnxyls.cn

TS:   [...arr].reverse();
来源：http://fm.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://xx.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ef.bjjhwx.cn

Ruby: arr.reverse
来源：http://za.chemitech.net.cn

C#:   list.Reverse();
来源：http://wv.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://xm.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://qu.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kb.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nj.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zt.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rx.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://bs.shxzukj.cn


<!-- 参考信息 -->