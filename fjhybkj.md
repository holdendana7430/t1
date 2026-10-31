代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jc.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://pa.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ma.colortex.cn

[B12] 跳出多层循环
来源：http://jv.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kb.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://av.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gk.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rd.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yt.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eh.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yk.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tq.hnjuh.cn

[B13] 判断是否为数字
来源：http://mf.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://zk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://ry.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ax.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bj.jctech888.com.cn

Java: x instanceof Number
来源：http://ag.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jr.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://jj.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://jr.colortex.cn

[B14] 判断值是否在集合内
来源：http://xd.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fq.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://si.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://nd.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://gz.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ys.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://un.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wd.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jp.9csxet.cn

[B15] 布尔运算与取反
来源：http://dn.gzmigu.cn

Py:   a and b or not c
来源：http://zn.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ml.panjiajie.cn

JS:   a && b || !c
来源：http://yj.asd995.cn

TS:   a && b || !c
来源：http://lh.muxihuayi.cn

Java: a && b || !c
来源：http://bu.9csxet.cn

Go:   a && b || !c
来源：http://ql.hahajie.cn

Ruby: a && b || !c
来源：http://of.jctech888.com.cn

C#:   a && b || !c
来源：http://cy.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ti.panjiajie.cn

Py:   if not data: return
来源：http://tx.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://un.szxytkj.cn

JS:   if (!data) return;
来源：http://xr.jctech888.com.cn

TS:   if (!data) return;
来源：http://kg.hnjuh.cn

Java: if (data == null) return;
来源：http://vd.jctech888.com.cn

Go:   if data == nil { return }
来源：http://mz.shtwfgs.cn

Ruby: return if data.nil?
来源：http://tm.521024.cn

C#:   if (data == null) return;
来源：http://gq.shxzukj.cn

================================================================================
来源：http://ma.nszjky.cn

C. 函数与作用域
来源：http://gp.bookmarksfly.cn

================================================================================
来源：http://yo.nszjky.cn

[C01] 定义函数
来源：http://ds.asd995.cn

Py:   def add(a, b): return a + b
来源：http://du.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oz.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://du.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hv.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lt.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uk.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://oi.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xi.yuntaijiaju.cn

[C02] 默认参数
来源：http://ks.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://ft.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hy.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://qy.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lj.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://up.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ex.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://tj.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://km.gzmigu.cn

[C03] 可变参数
来源：http://gu.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://lg.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ui.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kh.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nl.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mm.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://da.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ny.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yq.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://vz.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://za.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://md.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sb.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vz.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://zq.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://uk.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://on.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ga.colortex.cn

[C05] 返回多个值
来源：http://un.wgjwhj.cn

Py:   return a, b
来源：http://fv.panjiajie.cn

PHP:  return [$a, $b];
来源：http://cj.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jo.shxzskj.cn

TS:   return { a, b };
来源：http://oc.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nj.shtwfgs.cn

Go:   return a, b
来源：http://ag.nszjky.cn

Ruby: return a, b
来源：http://vl.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ha.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://xl.asd995.cn

Py:   square = lambda x: x * x
来源：http://qz.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ae.szsharing.cn

JS:   const square = x => x * x;
来源：http://bw.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://wn.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ip.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://su.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://re.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rj.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ai.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ok.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zu.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mj.colortex.cn

TS:   arr.map(String)
来源：http://tq.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gf.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ww.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://pi.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kj.haigaiapp.cn

[C08] 闭包
来源：http://cp.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zh.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yo.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mm.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rg.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ix.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://co.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zp.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bg.chemitech.net.cn

[C09] 递归
来源：http://nc.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jj.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qt.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lm.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hv.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hv.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zd.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fo.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rq.haigaiapp.cn

[C10] 变量作用域
来源：http://ca.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tk.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cj.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zb.huixiangedu.cn

TS:   同 JS
来源：http://xi.hahajie.cn

Java: 方法内为块级作用域
来源：http://kl.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://cs.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ix.szxytkj.cn

C#:   块级作用域
来源：http://am.huixiangedu.cn

[C11] 模块导入与导出
来源：http://uy.nszjky.cn

Py:   from module import func
来源：http://fl.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pj.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kh.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xx.huanxung.cn

Java: import java.util.List;
来源：http://zg.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rh.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ds.9csxet.cn

C#:   using System.Text;
来源：http://yu.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://yu.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://mp.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://uf.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://ga.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://nu.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hl.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://dn.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://lg.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rn.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://uy.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ei.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wf.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ii.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hn.hahajie.cn

Go:   func add(a, b int) int
来源：http://wv.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dj.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vs.9csxet.cn

[C14] 泛型函数
来源：http://xd.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ga.szxytkj.cn

PHP:  // 无泛型
来源：http://ui.521024.cn

JS:   // 无泛型
来源：http://te.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qu.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hh.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fd.gzmigu.cn

Ruby: # 无泛型
来源：http://mh.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zr.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://gt.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zf.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://hy.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dd.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://di.colortex.cn

Java: // 无解构
来源：http://kh.szsharing.cn

Go:   // 无解构
来源：http://gn.shxzukj.cn

Ruby: a, b = pair
来源：http://qs.hahajie.cn

C#:   var (a, b) = pair;
来源：http://de.nszjky.cn

[C16] 函数 / 方法重载
来源：http://jr.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zv.asd995.cn

PHP:  // 无重载
来源：http://pg.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gh.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://ig.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://hf.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://dz.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yc.panjiajie.cn

================================================================================
来源：http://yp.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://jy.asd995.cn

================================================================================
来源：http://av.521024.cn

[D01] 创建数组 / 列表
来源：http://ih.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zp.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oz.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bl.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ex.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://vo.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://cr.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ib.shxzskj.cn

[D02] 追加元素到末尾
来源：http://hx.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xc.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://or.hahajie.cn

JS:   arr.push(4);
来源：http://tw.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://mg.bjjhwx.cn

Java: list.add(4);
来源：http://st.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ah.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fy.hahajie.cn

C#:   list.Add(4);
来源：http://er.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://wn.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://ja.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oe.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qg.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://bu.lnxyls.cn

Java: list.add(0, 0);
来源：http://gk.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tz.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lm.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://fj.muxihuayi.cn

[D04] 删除元素
来源：http://of.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ww.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ky.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jg.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://vj.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hs.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rg.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hw.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qm.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ti.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gt.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gl.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://we.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://cn.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://hl.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://zj.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hs.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yt.szxytkj.cn

[D06] 数组长度
来源：http://xm.shxzskj.cn

Py:   len(arr)
来源：http://qp.gzmigu.cn

PHP:  count($arr);
来源：http://ek.hnjuh.cn

JS:   arr.length
来源：http://ws.wgjwhj.cn

TS:   arr.length
来源：http://js.huixiangedu.cn

Java: list.size();
来源：http://ev.9csxet.cn

Go:   len(arr)
来源：http://yn.szsharing.cn

Ruby: arr.length; arr.size
来源：http://gn.jctech888.com.cn

C#:   list.Count;
来源：http://jk.nicolike.cn

[D07] 切片 / 取子数组
来源：http://qn.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zc.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jo.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://mh.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://gc.9csxet.cn

Java: list.subList(1, 4);
来源：http://qp.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://kf.9csxet.cn

Ruby: arr[1, 3]
来源：http://ux.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://nm.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://of.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://sl.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://bk.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zj.lnxyls.cn

TS:   [...a, ...b];
来源：http://ds.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gg.bjjhwx.cn

Go:   append(a, b...)
来源：http://jb.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://gf.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://jo.bjjhwx.cn

[D09] 排序（升序）
来源：http://oa.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://sq.bookmarksfly.cn

PHP:  sort($arr);
来源：http://td.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nl.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bo.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fw.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ey.yuntaijiaju.cn

Ruby: arr.sort
来源：http://zl.szxytkj.cn

C#:   list.Sort();
来源：http://jn.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gk.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cf.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wj.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wg.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gj.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qm.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kx.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jf.panjiajie.cn

[D11] 反转数组
来源：http://dv.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jh.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://yt.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rq.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://km.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://cf.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://mf.9csxet.cn

Ruby: arr.reverse
来源：http://hy.jctech888.com.cn

C#:   list.Reverse();
来源：http://ft.shxzskj.cn

[D12] 查找元素下标
来源：http://td.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://by.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gk.9csxet.cn


<!-- 参考信息 -->