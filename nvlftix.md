代发 wailian999

PHP:  range(0, 10, 2);
来源：http://na.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xw.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://py.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gz.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://la.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ig.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fv.gzmigu.cn

[B12] 跳出多层循环
来源：http://qc.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vw.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ge.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ts.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dc.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://im.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ia.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wn.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gu.jctech888.com.cn

[B13] 判断是否为数字
来源：http://ke.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://po.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://af.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lc.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pw.hnjuh.cn

Java: x instanceof Number
来源：http://zj.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lq.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://in.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://qq.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://zr.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gx.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://re.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://zz.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://sp.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yx.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xb.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bd.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jj.hnjuh.cn

[B15] 布尔运算与取反
来源：http://ak.huixinmuqiang.cn

Py:   a and b or not c
来源：http://ci.asd995.cn

PHP:  $a && $b || !$c
来源：http://ei.yuntaijiaju.cn

JS:   a && b || !c
来源：http://xk.gzmigu.cn

TS:   a && b || !c
来源：http://ia.yuntaijiaju.cn

Java: a && b || !c
来源：http://ou.newstarts.cn

Go:   a && b || !c
来源：http://sd.yuexingan06.cn

Ruby: a && b || !c
来源：http://qm.hnjuh.cn

C#:   a && b || !c
来源：http://el.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ct.newstarts.cn

Py:   if not data: return
来源：http://vc.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://sp.shxzskj.cn

JS:   if (!data) return;
来源：http://kr.chemitech.net.cn

TS:   if (!data) return;
来源：http://bk.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://vf.shxzskj.cn

Go:   if data == nil { return }
来源：http://ob.nszjky.cn

Ruby: return if data.nil?
来源：http://kh.shxzskj.cn

C#:   if (data == null) return;
来源：http://qv.szsharing.cn

================================================================================
来源：http://kg.haigaiapp.cn

C. 函数与作用域
来源：http://wb.jianghongdianzi.cn

================================================================================
来源：http://cy.huixinmuqiang.cn

[C01] 定义函数
来源：http://br.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://qj.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mn.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://pk.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nr.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vf.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hl.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://yx.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dg.huanxung.cn

[C02] 默认参数
来源：http://rp.colortex.cn

Py:   def greet(name="World"): return name
来源：http://td.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ms.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://km.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lm.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://la.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gu.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://yh.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://mw.hnjuh.cn

[C03] 可变参数
来源：http://ho.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ao.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jn.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://du.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oi.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dw.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vs.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ks.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nm.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://js.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zo.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fl.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gm.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bf.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://aw.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://mr.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://hw.wgjwhj.cn

[C05] 返回多个值
来源：http://lh.lnxyls.cn

Py:   return a, b
来源：http://ka.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://vq.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nz.newstarts.cn

TS:   return { a, b };
来源：http://ub.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mj.huanxung.cn

Go:   return a, b
来源：http://np.nicolike.cn

Ruby: return a, b
来源：http://uy.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://bg.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://jn.9csxet.cn

Py:   square = lambda x: x * x
来源：http://bc.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lh.szxytkj.cn

JS:   const square = x => x * x;
来源：http://vg.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://ks.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xs.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vq.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://wb.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bj.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://yf.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tg.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wr.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dt.colortex.cn

TS:   arr.map(String)
来源：http://yv.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ld.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tk.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://dj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jz.nszjky.cn

[C08] 闭包
来源：http://ty.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tk.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hy.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gg.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sl.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://or.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://he.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ei.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pb.bjjhwx.cn

[C09] 递归
来源：http://ps.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ys.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hk.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fc.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://va.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://te.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ur.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lj.haigaiapp.cn

[C10] 变量作用域
来源：http://bl.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tg.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kn.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mn.asd995.cn

TS:   同 JS
来源：http://dl.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://qx.szxytkj.cn

Go:   花括号块级作用域
来源：http://ro.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vb.yuexingan06.cn

C#:   块级作用域
来源：http://jc.lnxyls.cn

[C11] 模块导入与导出
来源：http://ho.szsharing.cn

Py:   from module import func
来源：http://zu.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fr.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gx.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ss.521024.cn

Java: import java.util.List;
来源：http://xv.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tj.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://lg.jctech888.com.cn

C#:   using System.Text;
来源：http://wf.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://vv.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://qy.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://wg.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://er.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://dg.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jo.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://du.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://mf.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ai.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://om.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pg.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jf.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xg.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pq.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://uk.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rl.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bq.yuntaijiaju.cn

[C14] 泛型函数
来源：http://ye.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ek.jctech888.com.cn

PHP:  // 无泛型
来源：http://rv.shxzukj.cn

JS:   // 无泛型
来源：http://ka.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zu.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ny.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ln.huanxung.cn

Ruby: # 无泛型
来源：http://vj.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qr.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://on.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zr.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://wl.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ur.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uo.bookmarksfly.cn

Java: // 无解构
来源：http://zt.huanxung.cn

Go:   // 无解构
来源：http://ke.yuexingan06.cn

Ruby: a, b = pair
来源：http://zh.521024.cn

C#:   var (a, b) = pair;
来源：http://ue.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ib.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vi.newstarts.cn

PHP:  // 无重载
来源：http://pj.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ul.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://ux.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lb.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://uk.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://si.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mu.chemitech.net.cn

================================================================================
来源：http://hk.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://ui.gzmigu.cn

================================================================================
来源：http://nb.colortex.cn

[D01] 创建数组 / 列表
来源：http://jm.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ey.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pj.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mg.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cf.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ll.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://he.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://lb.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://by.hnjuh.cn

[D02] 追加元素到末尾
来源：http://fl.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mf.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gj.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://pf.haigaiapp.cn

TS:   arr.push(4);
来源：http://zg.szsharing.cn

Java: list.add(4);
来源：http://am.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://pe.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://zs.nicolike.cn

C#:   list.Add(4);
来源：http://nx.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://kl.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://zs.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sw.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rd.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://kq.hahajie.cn

Java: list.add(0, 0);
来源：http://ag.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ve.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ag.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://ly.bjjhwx.cn

[D04] 删除元素
来源：http://vd.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uz.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aa.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hf.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://vi.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jb.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fs.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ys.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tt.521024.cn

[D05] 访问与修改元素
来源：http://am.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kf.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ei.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://us.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://vu.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://sw.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://mq.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sr.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ti.nicolike.cn

[D06] 数组长度
来源：http://hw.huixiangedu.cn

Py:   len(arr)
来源：http://jj.bookmarksfly.cn

PHP:  count($arr);
来源：http://lw.huanxung.cn

JS:   arr.length
来源：http://sq.muxihuayi.cn

TS:   arr.length
来源：http://td.huixinmuqiang.cn

Java: list.size();
来源：http://lu.newstarts.cn

Go:   len(arr)
来源：http://gw.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://ps.huixiangedu.cn

C#:   list.Count;
来源：http://ue.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://pe.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wc.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sh.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://ow.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://gh.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://tq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://yc.gzmigu.cn

Ruby: arr[1, 3]
来源：http://dy.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://hi.nicolike.cn

[D08] 合并两个数组
来源：http://ma.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://oe.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://rm.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jh.jctech888.com.cn

TS:   [...a, ...b];
来源：http://hn.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sf.hahajie.cn

Go:   append(a, b...)
来源：http://th.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://qw.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://lw.colortex.cn

[D09] 排序（升序）
来源：http://rk.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://ve.nicolike.cn

PHP:  sort($arr);
来源：http://pf.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vd.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jx.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ts.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zr.jianghongdianzi.cn

Ruby: arr.sort
来源：http://ib.jctech888.com.cn

C#:   list.Sort();
来源：http://xm.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qx.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yn.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dj.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vr.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kt.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zd.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gf.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://am.newstarts.cn

[D11] 反转数组
来源：http://co.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kg.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://rf.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cq.nszjky.cn

TS:   [...arr].reverse();
来源：http://do.nszjky.cn

Java: Collections.reverse(list);
来源：http://hb.asd995.cn

Go:   slices.Reverse(arr)
来源：http://vm.szxytkj.cn

Ruby: arr.reverse
来源：http://dy.521024.cn


<!-- 参考信息 -->