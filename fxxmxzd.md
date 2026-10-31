代发 wailian999

[B13] 判断是否为数字
来源：http://hc.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://lv.asd995.cn

PHP:  is_numeric($x)
来源：http://ti.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kx.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dt.lnxyls.cn

Java: x instanceof Number
来源：http://pn.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ap.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://hr.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://md.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://pl.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://an.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://br.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://rs.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://tw.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oe.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ee.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zs.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bb.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://ua.hahajie.cn

Py:   a and b or not c
来源：http://jm.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://hd.wgjwhj.cn

JS:   a && b || !c
来源：http://vy.lnxyls.cn

TS:   a && b || !c
来源：http://xu.shxzskj.cn

Java: a && b || !c
来源：http://wl.huanxung.cn

Go:   a && b || !c
来源：http://pv.shxzskj.cn

Ruby: a && b || !c
来源：http://cm.huanxung.cn

C#:   a && b || !c
来源：http://us.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tu.szsharing.cn

Py:   if not data: return
来源：http://zt.colortex.cn

PHP:  if (!$data) { return; }
来源：http://uw.chemitech.net.cn

JS:   if (!data) return;
来源：http://zv.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://jh.huixiangedu.cn

Java: if (data == null) return;
来源：http://sg.haigaiapp.cn

Go:   if data == nil { return }
来源：http://ro.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://pv.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://rg.haigaiapp.cn

================================================================================
来源：http://bk.asd995.cn

C. 函数与作用域
来源：http://pu.panjiajie.cn

================================================================================
来源：http://vz.bjjhwx.cn

[C01] 定义函数
来源：http://zf.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://dg.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://dh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qn.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ta.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rb.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://zv.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pt.shxzskj.cn

[C02] 默认参数
来源：http://gb.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://sj.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yo.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://qz.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sn.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xq.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gd.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://gt.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://qn.9csxet.cn

[C03] 可变参数
来源：http://if.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://jv.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://um.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xe.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kw.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xa.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ez.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qa.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kv.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://nc.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://py.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://li.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xe.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ft.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://xw.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://cl.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://pw.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://bx.huanxung.cn

[C05] 返回多个值
来源：http://dd.nszjky.cn

Py:   return a, b
来源：http://yh.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://sl.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ex.wgjwhj.cn

TS:   return { a, b };
来源：http://jw.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zb.panjiajie.cn

Go:   return a, b
来源：http://pl.shxzukj.cn

Ruby: return a, b
来源：http://uc.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://oa.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://av.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://aa.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://na.asd995.cn

JS:   const square = x => x * x;
来源：http://gs.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://mz.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vk.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pg.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ox.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ic.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://cn.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rr.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ra.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sx.haigaiapp.cn

TS:   arr.map(String)
来源：http://hj.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sy.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gc.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://ek.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ry.nszjky.cn

[C08] 闭包
来源：http://kt.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vs.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yh.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dl.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pw.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wq.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gb.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dh.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tq.muxihuayi.cn

[C09] 递归
来源：http://qh.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qd.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zw.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xb.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rj.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xq.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dy.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ey.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fq.shxzskj.cn

[C10] 变量作用域
来源：http://ly.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rv.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wc.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rn.bjjhwx.cn

TS:   同 JS
来源：http://hd.szxytkj.cn

Java: 方法内为块级作用域
来源：http://gk.huixiangedu.cn

Go:   花括号块级作用域
来源：http://qo.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kt.shxzskj.cn

C#:   块级作用域
来源：http://vr.asd995.cn

[C11] 模块导入与导出
来源：http://ac.szsharing.cn

Py:   from module import func
来源：http://xc.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://si.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hs.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://if.colortex.cn

Java: import java.util.List;
来源：http://uc.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://el.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://pk.szsharing.cn

C#:   using System.Text;
来源：http://bh.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://wt.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://oq.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://pd.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://zq.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://du.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qk.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://fw.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://wd.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sm.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://hc.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fk.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://en.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://on.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fi.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ga.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://vo.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yk.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vd.chemitech.net.cn

[C14] 泛型函数
来源：http://uh.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wz.gzmigu.cn

PHP:  // 无泛型
来源：http://re.panjiajie.cn

JS:   // 无泛型
来源：http://ws.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lc.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://na.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yd.9csxet.cn

Ruby: # 无泛型
来源：http://wm.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://la.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://af.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gc.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://sm.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pz.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gh.hahajie.cn

Java: // 无解构
来源：http://lu.shxzskj.cn

Go:   // 无解构
来源：http://xl.huanxung.cn

Ruby: a, b = pair
来源：http://nk.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://tr.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://dh.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tc.panjiajie.cn

PHP:  // 无重载
来源：http://ti.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gh.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://fe.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qu.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://on.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://ka.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bv.panjiajie.cn

================================================================================
来源：http://yl.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://ot.jianghongdianzi.cn

================================================================================
来源：http://dh.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://nr.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cp.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bv.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dd.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://td.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ge.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://yx.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://ji.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ed.nszjky.cn

[D02] 追加元素到末尾
来源：http://ew.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dx.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xu.wgjwhj.cn

JS:   arr.push(4);
来源：http://xi.szsharing.cn

TS:   arr.push(4);
来源：http://at.huanxung.cn

Java: list.add(4);
来源：http://vm.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://ie.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://es.panjiajie.cn

C#:   list.Add(4);
来源：http://vp.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://vl.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://mh.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zw.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kc.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ke.shxzukj.cn

Java: list.add(0, 0);
来源：http://yv.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dx.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://su.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://ln.hnjuh.cn

[D04] 删除元素
来源：http://gt.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ee.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gl.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gp.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://sm.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ik.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bi.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nx.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bn.shxzukj.cn

[D05] 访问与修改元素
来源：http://tp.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fa.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://if.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yl.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://ol.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://op.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://xe.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aj.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iw.asd995.cn

[D06] 数组长度
来源：http://mj.muxihuayi.cn

Py:   len(arr)
来源：http://ju.muxihuayi.cn

PHP:  count($arr);
来源：http://my.haigaiapp.cn

JS:   arr.length
来源：http://jd.yuntaijiaju.cn

TS:   arr.length
来源：http://mf.huanxung.cn

Java: list.size();
来源：http://yc.chemitech.net.cn

Go:   len(arr)
来源：http://mh.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://oc.bjjhwx.cn

C#:   list.Count;
来源：http://nf.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://vh.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ys.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tz.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://ik.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://qw.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://ft.521024.cn

Go:   arr[1:4]
来源：http://za.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://im.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://ic.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://le.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://rr.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://ui.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qg.nicolike.cn

TS:   [...a, ...b];
来源：http://re.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oq.hnjuh.cn

Go:   append(a, b...)
来源：http://wm.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://mc.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://sz.chemitech.net.cn

[D09] 排序（升序）
来源：http://pk.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://er.nicolike.cn

PHP:  sort($arr);
来源：http://bt.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jb.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kp.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uu.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zp.wgjwhj.cn

Ruby: arr.sort
来源：http://ey.huixinmuqiang.cn

C#:   list.Sort();
来源：http://tq.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sy.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vm.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jj.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ea.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ho.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qg.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jh.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cq.hahajie.cn

[D11] 反转数组
来源：http://lw.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://il.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yv.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://me.asd995.cn

TS:   [...arr].reverse();
来源：http://ev.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://fm.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://sk.szsharing.cn

Ruby: arr.reverse
来源：http://bq.szsharing.cn

C#:   list.Reverse();
来源：http://kr.newstarts.cn

[D12] 查找元素下标
来源：http://ru.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://np.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xr.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kf.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cw.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zv.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://tq.newstarts.cn

Ruby: arr.index(x)
来源：http://ux.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://wo.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://jx.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xr.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hb.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://bs.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://bn.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rp.jianghongdianzi.cn


<!-- 参考信息 -->