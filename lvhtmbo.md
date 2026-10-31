代发 wailian999

C#:   x is int or double or decimal
来源：http://or.hahajie.cn

[B14] 判断值是否在集合内
来源：http://vx.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bg.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sg.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ut.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://fw.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rn.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kn.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xy.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pv.panjiajie.cn

[B15] 布尔运算与取反
来源：http://fu.panjiajie.cn

Py:   a and b or not c
来源：http://pb.szsharing.cn

PHP:  $a && $b || !$c
来源：http://zh.nicolike.cn

JS:   a && b || !c
来源：http://ha.shxzukj.cn

TS:   a && b || !c
来源：http://zp.haigaiapp.cn

Java: a && b || !c
来源：http://kc.szsharing.cn

Go:   a && b || !c
来源：http://mn.panjiajie.cn

Ruby: a && b || !c
来源：http://dq.hnjuh.cn

C#:   a && b || !c
来源：http://ac.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ws.lnxyls.cn

Py:   if not data: return
来源：http://go.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://wp.haigaiapp.cn

JS:   if (!data) return;
来源：http://vr.shxzukj.cn

TS:   if (!data) return;
来源：http://ja.shxzskj.cn

Java: if (data == null) return;
来源：http://fh.huanxung.cn

Go:   if data == nil { return }
来源：http://gh.lnxyls.cn

Ruby: return if data.nil?
来源：http://fg.9csxet.cn

C#:   if (data == null) return;
来源：http://tc.bookmarksfly.cn

================================================================================
来源：http://db.521024.cn

C. 函数与作用域
来源：http://ic.haigaiapp.cn

================================================================================
来源：http://fp.szxytkj.cn

[C01] 定义函数
来源：http://su.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://oc.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wx.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ws.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rp.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jr.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gk.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ou.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://df.bjjhwx.cn

[C02] 默认参数
来源：http://bx.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://gb.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bf.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://hz.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eg.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ky.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dq.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://kd.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://sd.wgjwhj.cn

[C03] 可变参数
来源：http://mm.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://af.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oy.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uu.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://df.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ur.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gp.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ly.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yq.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://fc.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ys.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ks.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fs.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nb.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://hh.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://mq.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ku.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://oy.szxytkj.cn

[C05] 返回多个值
来源：http://vc.bookmarksfly.cn

Py:   return a, b
来源：http://wa.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://gg.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zd.newstarts.cn

TS:   return { a, b };
来源：http://zh.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jb.shxzukj.cn

Go:   return a, b
来源：http://ck.hnjuh.cn

Ruby: return a, b
来源：http://oj.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ln.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://wm.hahajie.cn

Py:   square = lambda x: x * x
来源：http://dv.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://or.newstarts.cn

JS:   const square = x => x * x;
来源：http://ey.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://kw.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sw.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hs.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://vr.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gz.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://my.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qa.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gy.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yl.huixiangedu.cn

TS:   arr.map(String)
来源：http://um.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jc.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hb.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://xx.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://te.shtwfgs.cn

[C08] 闭包
来源：http://wq.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://db.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vv.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sh.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ra.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jm.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mk.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mt.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lf.haigaiapp.cn

[C09] 递归
来源：http://rb.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uy.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gw.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hw.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://th.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uw.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xg.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aw.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mj.hahajie.cn

[C10] 变量作用域
来源：http://no.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://up.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://my.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hl.hahajie.cn

TS:   同 JS
来源：http://jw.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://uf.szsharing.cn

Go:   花括号块级作用域
来源：http://cx.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kl.521024.cn

C#:   块级作用域
来源：http://by.chemitech.net.cn

[C11] 模块导入与导出
来源：http://sy.hahajie.cn

Py:   from module import func
来源：http://ox.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tl.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://db.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dx.huanxung.cn

Java: import java.util.List;
来源：http://vo.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mm.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://dq.huixinmuqiang.cn

C#:   using System.Text;
来源：http://zg.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://xj.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://in.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://xw.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://fe.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://bm.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://im.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://bp.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://qv.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tf.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://ta.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nw.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cy.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://se.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vl.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uq.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://uj.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ed.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nr.szsharing.cn

[C14] 泛型函数
来源：http://aq.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xd.huanxung.cn

PHP:  // 无泛型
来源：http://uk.szsharing.cn

JS:   // 无泛型
来源：http://jh.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zo.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gj.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sg.hnjuh.cn

Ruby: # 无泛型
来源：http://at.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sd.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://qu.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mb.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://jh.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yu.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ol.shxzskj.cn

Java: // 无解构
来源：http://wc.hahajie.cn

Go:   // 无解构
来源：http://sq.haigaiapp.cn

Ruby: a, b = pair
来源：http://eh.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://zw.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://vz.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wa.bookmarksfly.cn

PHP:  // 无重载
来源：http://pi.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://af.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://nt.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://le.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://jy.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://vc.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ys.shxzskj.cn

================================================================================
来源：http://hz.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://vh.huanxung.cn

================================================================================
来源：http://kn.9csxet.cn

[D01] 创建数组 / 列表
来源：http://nr.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qz.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iu.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xk.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://it.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ok.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://mo.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://lc.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qt.hahajie.cn

[D02] 追加元素到末尾
来源：http://kt.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ju.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lx.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://mh.chemitech.net.cn

TS:   arr.push(4);
来源：http://rj.nicolike.cn

Java: list.add(4);
来源：http://zr.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://pg.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://nu.bookmarksfly.cn

C#:   list.Add(4);
来源：http://je.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://en.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://xo.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ot.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kq.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://im.yuexingan06.cn

Java: list.add(0, 0);
来源：http://hq.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://de.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zq.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ns.bookmarksfly.cn

[D04] 删除元素
来源：http://wb.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nf.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yb.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hl.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://rh.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://je.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://km.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nb.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oh.panjiajie.cn

[D05] 访问与修改元素
来源：http://se.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yn.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://be.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zl.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rg.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://sd.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://um.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ao.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iq.panjiajie.cn

[D06] 数组长度
来源：http://cn.521024.cn

Py:   len(arr)
来源：http://ta.9csxet.cn

PHP:  count($arr);
来源：http://pg.colortex.cn

JS:   arr.length
来源：http://pv.shtwfgs.cn

TS:   arr.length
来源：http://gg.shtwfgs.cn

Java: list.size();
来源：http://ab.huanxung.cn

Go:   len(arr)
来源：http://gc.521024.cn

Ruby: arr.length; arr.size
来源：http://zd.asd995.cn

C#:   list.Count;
来源：http://cj.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://ib.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mx.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hu.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://qx.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://tr.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://tt.bjjhwx.cn

Go:   arr[1:4]
来源：http://le.shxzskj.cn

Ruby: arr[1, 3]
来源：http://xz.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://cn.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://dc.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://rv.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://cc.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lh.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ym.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lt.wgjwhj.cn

Go:   append(a, b...)
来源：http://nl.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://oe.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://ht.colortex.cn

[D09] 排序（升序）
来源：http://hz.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://ba.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ls.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hp.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yp.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jg.panjiajie.cn

Ruby: arr.sort
来源：http://ld.hahajie.cn

C#:   list.Sort();
来源：http://ff.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tj.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mm.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kb.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bg.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zv.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://or.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fx.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://de.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ix.haigaiapp.cn

[D11] 反转数组
来源：http://wl.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kn.521024.cn

PHP:  array_reverse($arr);
来源：http://ga.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://by.panjiajie.cn

TS:   [...arr].reverse();
来源：http://zh.hahajie.cn

Java: Collections.reverse(list);
来源：http://pj.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://pm.szsharing.cn

Ruby: arr.reverse
来源：http://jv.huanxung.cn

C#:   list.Reverse();
来源：http://cx.haigaiapp.cn

[D12] 查找元素下标
来源：http://iy.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://vj.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oe.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hs.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nu.521024.cn

Go:   slices.Index(arr, x)
来源：http://gb.wgjwhj.cn

Ruby: arr.index(x)
来源：http://yl.9csxet.cn

C#:   list.IndexOf(x);
来源：http://gy.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://py.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rk.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wz.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://kt.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://wu.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gv.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sv.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gr.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zd.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://zs.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ps.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mc.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://ce.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ji.huixiangedu.cn


<!-- 参考信息 -->