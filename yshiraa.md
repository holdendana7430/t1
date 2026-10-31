代发 wailian999

[B13] 判断是否为数字
来源：http://nc.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://mj.newstarts.cn

PHP:  is_numeric($x)
来源：http://xk.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xg.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jb.bjjhwx.cn

Java: x instanceof Number
来源：http://ip.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nh.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://er.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ww.nszjky.cn

[B14] 判断值是否在集合内
来源：http://ve.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vf.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qx.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://pn.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://df.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vg.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mt.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mo.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ry.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://my.shxzskj.cn

Py:   a and b or not c
来源：http://ab.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://kd.muxihuayi.cn

JS:   a && b || !c
来源：http://ox.panjiajie.cn

TS:   a && b || !c
来源：http://eh.bjjhwx.cn

Java: a && b || !c
来源：http://hg.bookmarksfly.cn

Go:   a && b || !c
来源：http://ub.shxzskj.cn

Ruby: a && b || !c
来源：http://sr.shtwfgs.cn

C#:   a && b || !c
来源：http://ni.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fx.bjjhwx.cn

Py:   if not data: return
来源：http://wt.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://lx.newstarts.cn

JS:   if (!data) return;
来源：http://vf.huixiangedu.cn

TS:   if (!data) return;
来源：http://jg.nicolike.cn

Java: if (data == null) return;
来源：http://ip.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://xg.yuexingan06.cn

Ruby: return if data.nil?
来源：http://to.521024.cn

C#:   if (data == null) return;
来源：http://po.shxzukj.cn

================================================================================
来源：http://gh.huixiangedu.cn

C. 函数与作用域
来源：http://jr.szsharing.cn

================================================================================
来源：http://vz.hnjuh.cn

[C01] 定义函数
来源：http://fk.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://ea.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ia.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lo.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iz.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aa.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ux.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fr.9csxet.cn

[C02] 默认参数
来源：http://kf.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://xq.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tt.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://mi.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rb.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gi.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mb.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ld.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://jd.9csxet.cn

[C03] 可变参数
来源：http://mo.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://wl.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wt.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qb.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uf.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zl.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bw.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qn.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://zi.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vn.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://az.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lb.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wk.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://xq.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://wm.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://nv.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://rt.jctech888.com.cn

[C05] 返回多个值
来源：http://ns.newstarts.cn

Py:   return a, b
来源：http://ug.shxzukj.cn

PHP:  return [$a, $b];
来源：http://kq.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yi.huixinmuqiang.cn

TS:   return { a, b };
来源：http://jj.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pd.jctech888.com.cn

Go:   return a, b
来源：http://ue.haigaiapp.cn

Ruby: return a, b
来源：http://jt.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://mv.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://qp.huanxung.cn

Py:   square = lambda x: x * x
来源：http://pb.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ej.colortex.cn

JS:   const square = x => x * x;
来源：http://rj.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://sn.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dt.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aa.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://cj.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cz.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://nt.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mn.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ls.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://be.hnjuh.cn

TS:   arr.map(String)
来源：http://ih.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cl.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uc.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://ra.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ly.szsharing.cn

[C08] 闭包
来源：http://wz.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ev.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uv.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oq.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yc.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://op.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bb.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nt.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ez.521024.cn

[C09] 递归
来源：http://lk.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hu.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wp.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mm.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lg.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gv.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gw.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qf.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rk.newstarts.cn

[C10] 变量作用域
来源：http://gi.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://is.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xt.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uu.shxzskj.cn

TS:   同 JS
来源：http://sz.newstarts.cn

Java: 方法内为块级作用域
来源：http://ia.chemitech.net.cn

Go:   花括号块级作用域
来源：http://lq.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rd.szsharing.cn

C#:   块级作用域
来源：http://rm.nicolike.cn

[C11] 模块导入与导出
来源：http://mw.szxytkj.cn

Py:   from module import func
来源：http://ok.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://go.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ca.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://az.jctech888.com.cn

Java: import java.util.List;
来源：http://zq.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oz.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://se.szsharing.cn

C#:   using System.Text;
来源：http://zb.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://wo.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://jo.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://nn.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ce.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://kb.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zt.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://me.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://kb.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wi.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ky.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vn.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wi.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yl.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wl.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://ak.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jb.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uy.huanxung.cn

[C14] 泛型函数
来源：http://sf.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cy.newstarts.cn

PHP:  // 无泛型
来源：http://ji.huixinmuqiang.cn

JS:   // 无泛型
来源：http://tw.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ep.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ha.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lx.nszjky.cn

Ruby: # 无泛型
来源：http://cz.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uq.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://gr.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lx.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ts.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mo.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qw.shxzskj.cn

Java: // 无解构
来源：http://xh.colortex.cn

Go:   // 无解构
来源：http://qn.colortex.cn

Ruby: a, b = pair
来源：http://wo.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://eg.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://ut.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kz.shtwfgs.cn

PHP:  // 无重载
来源：http://wt.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jg.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://yn.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wq.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://ty.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://lm.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xk.colortex.cn

================================================================================
来源：http://bj.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://xl.huanxung.cn

================================================================================
来源：http://ci.521024.cn

[D01] 创建数组 / 列表
来源：http://yq.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zn.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://be.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://it.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yh.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hb.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://kk.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://gq.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uy.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://gm.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sb.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://br.muxihuayi.cn

JS:   arr.push(4);
来源：http://ws.yuexingan06.cn

TS:   arr.push(4);
来源：http://yu.haigaiapp.cn

Java: list.add(4);
来源：http://ua.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://hl.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://qj.hnjuh.cn

C#:   list.Add(4);
来源：http://sa.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ab.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://md.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qr.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://id.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://fx.shxzukj.cn

Java: list.add(0, 0);
来源：http://lg.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://js.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zl.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://ex.9csxet.cn

[D04] 删除元素
来源：http://ca.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xv.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mp.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ov.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://dg.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ys.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zb.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xc.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ey.gzmigu.cn

[D05] 访问与修改元素
来源：http://wo.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://no.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ca.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lm.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://kx.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://kq.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://cp.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ax.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lr.hahajie.cn

[D06] 数组长度
来源：http://nm.chemitech.net.cn

Py:   len(arr)
来源：http://hh.wgjwhj.cn

PHP:  count($arr);
来源：http://ts.jctech888.com.cn

JS:   arr.length
来源：http://ys.jianghongdianzi.cn

TS:   arr.length
来源：http://gj.wgjwhj.cn

Java: list.size();
来源：http://fr.hnjuh.cn

Go:   len(arr)
来源：http://hx.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://nl.muxihuayi.cn

C#:   list.Count;
来源：http://jd.9csxet.cn

[D07] 切片 / 取子数组
来源：http://yq.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eh.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ap.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://td.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://cy.asd995.cn

Java: list.subList(1, 4);
来源：http://tj.jctech888.com.cn

Go:   arr[1:4]
来源：http://wh.shxzskj.cn

Ruby: arr[1, 3]
来源：http://vs.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://bn.chemitech.net.cn

[D08] 合并两个数组
来源：http://cm.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://to.colortex.cn

PHP:  array_merge($a, $b);
来源：http://bx.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kc.newstarts.cn

TS:   [...a, ...b];
来源：http://eg.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://js.nicolike.cn

Go:   append(a, b...)
来源：http://bm.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://wz.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://vu.hnjuh.cn

[D09] 排序（升序）
来源：http://mg.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://zp.shxzukj.cn

PHP:  sort($arr);
来源：http://vx.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pv.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ko.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://az.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xi.bjjhwx.cn

Ruby: arr.sort
来源：http://em.colortex.cn

C#:   list.Sort();
来源：http://fl.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xv.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rq.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://th.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oe.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cp.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lo.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://be.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gv.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://st.hahajie.cn

[D11] 反转数组
来源：http://gi.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://in.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://io.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://li.521024.cn

TS:   [...arr].reverse();
来源：http://lk.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://zz.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://vw.szsharing.cn

Ruby: arr.reverse
来源：http://bz.wgjwhj.cn

C#:   list.Reverse();
来源：http://lz.lnxyls.cn

[D12] 查找元素下标
来源：http://ax.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://ee.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uk.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tt.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cp.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ny.colortex.cn

Go:   slices.Index(arr, x)
来源：http://vh.shxzukj.cn

Ruby: arr.index(x)
来源：http://ra.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://tw.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ck.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kr.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oc.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://du.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://rm.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qw.szxytkj.cn


<!-- 参考信息 -->