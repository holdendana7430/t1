代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://hr.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tq.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qa.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://np.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ae.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zz.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mc.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sj.9csxet.cn

[B13] 判断是否为数字
来源：http://wh.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://hf.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ww.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xs.bookmarksfly.cn

Java: x instanceof Number
来源：http://rk.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tu.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://gt.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://no.521024.cn

[B14] 判断值是否在集合内
来源：http://mc.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ft.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zz.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://rn.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://mh.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vr.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kh.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jj.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fu.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://wn.bookmarksfly.cn

Py:   a and b or not c
来源：http://ly.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ix.wgjwhj.cn

JS:   a && b || !c
来源：http://nk.521024.cn

TS:   a && b || !c
来源：http://qx.haigaiapp.cn

Java: a && b || !c
来源：http://ou.hnjuh.cn

Go:   a && b || !c
来源：http://xi.muxihuayi.cn

Ruby: a && b || !c
来源：http://pr.shxzskj.cn

C#:   a && b || !c
来源：http://mh.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nt.newstarts.cn

Py:   if not data: return
来源：http://bf.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://ez.newstarts.cn

JS:   if (!data) return;
来源：http://mu.nszjky.cn

TS:   if (!data) return;
来源：http://ws.hnjuh.cn

Java: if (data == null) return;
来源：http://wm.hahajie.cn

Go:   if data == nil { return }
来源：http://ju.szsharing.cn

Ruby: return if data.nil?
来源：http://nc.9csxet.cn

C#:   if (data == null) return;
来源：http://tc.bjjhwx.cn

================================================================================
来源：http://jc.521024.cn

C. 函数与作用域
来源：http://wm.huanxung.cn

================================================================================
来源：http://qy.521024.cn

[C01] 定义函数
来源：http://zp.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://yf.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://ix.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dw.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://st.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qh.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://lq.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ot.nicolike.cn

[C02] 默认参数
来源：http://cs.asd995.cn

Py:   def greet(name="World"): return name
来源：http://pk.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lr.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://yi.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mf.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rd.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ja.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ru.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gm.hnjuh.cn

[C03] 可变参数
来源：http://aw.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://nf.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mb.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ew.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cl.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fg.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qp.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://we.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zx.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://jq.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fi.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ml.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jg.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fh.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qy.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ko.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://sh.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://yk.9csxet.cn

[C05] 返回多个值
来源：http://ud.haigaiapp.cn

Py:   return a, b
来源：http://qz.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://sy.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zk.chemitech.net.cn

TS:   return { a, b };
来源：http://rz.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rs.colortex.cn

Go:   return a, b
来源：http://id.hnjuh.cn

Ruby: return a, b
来源：http://xu.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://qc.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://vq.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://rf.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xt.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://bd.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://tk.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rr.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cb.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://qi.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tv.9csxet.cn

[C07] 把函数作为参数传入
来源：http://vw.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uj.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ts.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fr.muxihuayi.cn

TS:   arr.map(String)
来源：http://ne.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://is.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mo.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://fo.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ur.shtwfgs.cn

[C08] 闭包
来源：http://fr.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dv.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pt.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rm.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wg.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://et.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ep.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tk.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xp.yuexingan06.cn

[C09] 递归
来源：http://wr.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ia.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zz.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bo.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://av.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dx.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ed.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pq.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://op.yuntaijiaju.cn

[C10] 变量作用域
来源：http://mu.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vm.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://np.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://th.haigaiapp.cn

TS:   同 JS
来源：http://fl.hahajie.cn

Java: 方法内为块级作用域
来源：http://jv.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://xr.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aj.hnjuh.cn

C#:   块级作用域
来源：http://mi.chemitech.net.cn

[C11] 模块导入与导出
来源：http://jc.gzmigu.cn

Py:   from module import func
来源：http://ye.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cy.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lb.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zy.shtwfgs.cn

Java: import java.util.List;
来源：http://ur.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ht.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://vh.bookmarksfly.cn

C#:   using System.Text;
来源：http://qr.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://nx.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://qv.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://vx.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://pt.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://fn.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kt.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://xz.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://ca.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://he.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://ju.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bo.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vh.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dc.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wn.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ih.szsharing.cn

Go:   func add(a, b int) int
来源：http://da.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uu.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uk.haigaiapp.cn

[C14] 泛型函数
来源：http://xe.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://za.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://fq.huixinmuqiang.cn

JS:   // 无泛型
来源：http://th.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wv.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://if.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gg.panjiajie.cn

Ruby: # 无泛型
来源：http://pp.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fq.huanxung.cn

[C15] 解构 / 展开参数
来源：http://yf.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tt.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ve.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rw.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bu.colortex.cn

Java: // 无解构
来源：http://pg.shxzukj.cn

Go:   // 无解构
来源：http://fd.shxzukj.cn

Ruby: a, b = pair
来源：http://mt.newstarts.cn

C#:   var (a, b) = pair;
来源：http://hc.asd995.cn

[C16] 函数 / 方法重载
来源：http://ke.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sx.shtwfgs.cn

PHP:  // 无重载
来源：http://pg.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gg.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://vg.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vn.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://pm.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://kt.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://te.asd995.cn

================================================================================
来源：http://mc.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ur.muxihuayi.cn

================================================================================
来源：http://rl.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://th.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dk.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cm.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vq.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jd.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ub.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://fd.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ph.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zy.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://aj.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vv.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fj.hahajie.cn

JS:   arr.push(4);
来源：http://pq.muxihuayi.cn

TS:   arr.push(4);
来源：http://cy.muxihuayi.cn

Java: list.add(4);
来源：http://rh.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://fb.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://qo.bjjhwx.cn

C#:   list.Add(4);
来源：http://cx.asd995.cn

[D03] 在指定位置插入元素
来源：http://qi.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://me.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kx.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jj.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ov.haigaiapp.cn

Java: list.add(0, 0);
来源：http://rc.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pr.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uj.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://ob.shxzskj.cn

[D04] 删除元素
来源：http://yb.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uk.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rd.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://fv.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wl.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fo.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rf.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://id.shtwfgs.cn

[D05] 访问与修改元素
来源：http://xl.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zm.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pw.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bj.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://dl.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://xu.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://ht.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xc.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rc.521024.cn

[D06] 数组长度
来源：http://kt.jctech888.com.cn

Py:   len(arr)
来源：http://pi.hahajie.cn

PHP:  count($arr);
来源：http://rz.521024.cn

JS:   arr.length
来源：http://mh.chemitech.net.cn

TS:   arr.length
来源：http://ol.nicolike.cn

Java: list.size();
来源：http://yd.yuexingan06.cn

Go:   len(arr)
来源：http://sm.nicolike.cn

Ruby: arr.length; arr.size
来源：http://wo.jianghongdianzi.cn

C#:   list.Count;
来源：http://xs.hahajie.cn

[D07] 切片 / 取子数组
来源：http://as.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yn.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://js.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://ad.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://lw.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://vp.bookmarksfly.cn

Go:   arr[1:4]
来源：http://qj.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://pd.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://cf.szxytkj.cn

[D08] 合并两个数组
来源：http://ys.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://fa.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://fm.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://em.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://sa.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mk.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ej.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://yj.521024.cn

C#:   a.Concat(b).ToList()
来源：http://et.nszjky.cn

[D09] 排序（升序）
来源：http://dl.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://kh.huixiangedu.cn

PHP:  sort($arr);
来源：http://ff.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rj.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dp.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://um.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tu.gzmigu.cn

Ruby: arr.sort
来源：http://gx.chemitech.net.cn

C#:   list.Sort();
来源：http://ot.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sf.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mh.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jw.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ly.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dq.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jg.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sk.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jy.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://is.hahajie.cn

[D11] 反转数组
来源：http://re.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ny.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://qb.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fn.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://sp.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://ju.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://nr.bjjhwx.cn

Ruby: arr.reverse
来源：http://gs.muxihuayi.cn

C#:   list.Reverse();
来源：http://fz.hahajie.cn

[D12] 查找元素下标
来源：http://yj.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://ua.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mc.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wb.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://or.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ub.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://zh.hahajie.cn


<!-- 参考信息 -->