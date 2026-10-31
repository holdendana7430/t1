代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dx.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xa.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://hd.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://wa.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://tq.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wh.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gg.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ev.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bx.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://wm.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zj.hahajie.cn

[B12] 跳出多层循环
来源：http://bp.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ou.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://no.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kt.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jl.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mo.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wy.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fg.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yt.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://yd.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ie.hahajie.cn

PHP:  is_numeric($x)
来源：http://xs.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sf.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qn.9csxet.cn

Java: x instanceof Number
来源：http://rv.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cp.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://nk.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://rm.hahajie.cn

[B14] 判断值是否在集合内
来源：http://nh.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ox.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xt.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://lh.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://rn.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rf.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hh.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vx.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tm.shxzskj.cn

[B15] 布尔运算与取反
来源：http://tc.huixiangedu.cn

Py:   a and b or not c
来源：http://gb.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://fs.hnjuh.cn

JS:   a && b || !c
来源：http://aa.521024.cn

TS:   a && b || !c
来源：http://sc.9csxet.cn

Java: a && b || !c
来源：http://bk.shxzukj.cn

Go:   a && b || !c
来源：http://jf.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://zd.9csxet.cn

C#:   a && b || !c
来源：http://ec.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tu.huanxung.cn

Py:   if not data: return
来源：http://ve.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://sr.lnxyls.cn

JS:   if (!data) return;
来源：http://os.jctech888.com.cn

TS:   if (!data) return;
来源：http://hk.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://tz.hahajie.cn

Go:   if data == nil { return }
来源：http://bp.yuexingan06.cn

Ruby: return if data.nil?
来源：http://wb.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://nn.muxihuayi.cn

================================================================================
来源：http://qx.haigaiapp.cn

C. 函数与作用域
来源：http://me.521024.cn

================================================================================
来源：http://zi.colortex.cn

[C01] 定义函数
来源：http://xa.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://yk.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ln.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://an.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://md.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gm.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bl.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://ah.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ah.szxytkj.cn

[C02] 默认参数
来源：http://jc.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://sh.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vm.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://vl.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tz.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tp.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ey.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://nc.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://yc.bookmarksfly.cn

[C03] 可变参数
来源：http://sd.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://ea.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ow.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://al.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wv.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bf.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ue.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nw.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jo.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://lj.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ut.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tz.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ez.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wi.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://uc.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://dq.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://tl.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://hl.shxzskj.cn

[C05] 返回多个值
来源：http://hv.huixiangedu.cn

Py:   return a, b
来源：http://dv.shxzskj.cn

PHP:  return [$a, $b];
来源：http://yk.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kt.521024.cn

TS:   return { a, b };
来源：http://gn.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nx.wgjwhj.cn

Go:   return a, b
来源：http://ti.szxytkj.cn

Ruby: return a, b
来源：http://bl.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://xq.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ga.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://qe.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fc.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://vi.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://bw.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zw.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ub.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ou.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kn.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ta.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kr.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kc.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ld.haigaiapp.cn

TS:   arr.map(String)
来源：http://gj.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vp.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://as.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://ax.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iz.yuexingan06.cn

[C08] 闭包
来源：http://we.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nz.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ia.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ii.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vd.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vd.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vb.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oc.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oc.panjiajie.cn

[C09] 递归
来源：http://bu.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bq.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ly.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wz.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fn.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lo.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yl.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hp.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ij.521024.cn

[C10] 变量作用域
来源：http://qu.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://au.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mr.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wr.jianghongdianzi.cn

TS:   同 JS
来源：http://cb.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://qc.bjjhwx.cn

Go:   花括号块级作用域
来源：http://bm.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yh.colortex.cn

C#:   块级作用域
来源：http://wk.nszjky.cn

[C11] 模块导入与导出
来源：http://yk.9csxet.cn

Py:   from module import func
来源：http://ip.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ip.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dx.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cn.huixinmuqiang.cn

Java: import java.util.List;
来源：http://tx.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ju.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ze.chemitech.net.cn

C#:   using System.Text;
来源：http://ww.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://zn.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://jd.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://js.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://ck.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ha.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gf.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://jo.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://qn.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lz.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://lu.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rt.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xo.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ot.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uo.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9csxet.cn

Go:   func add(a, b int) int
来源：http://uf.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xv.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yk.yuntaijiaju.cn

[C14] 泛型函数
来源：http://df.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fp.chemitech.net.cn

PHP:  // 无泛型
来源：http://zu.bookmarksfly.cn

JS:   // 无泛型
来源：http://ew.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ig.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mu.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ne.jctech888.com.cn

Ruby: # 无泛型
来源：http://mh.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qk.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://ij.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://od.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://cw.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xq.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oj.muxihuayi.cn

Java: // 无解构
来源：http://pu.huixiangedu.cn

Go:   // 无解构
来源：http://vz.nszjky.cn

Ruby: a, b = pair
来源：http://hd.nszjky.cn

C#:   var (a, b) = pair;
来源：http://px.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://du.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cu.bjjhwx.cn

PHP:  // 无重载
来源：http://fg.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oi.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://gt.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qt.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://rx.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://jg.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gi.bjjhwx.cn

================================================================================
来源：http://gp.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://bo.hahajie.cn

================================================================================
来源：http://fq.newstarts.cn

[D01] 创建数组 / 列表
来源：http://hc.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jm.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nn.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uc.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fz.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ke.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://ok.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://dv.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.panjiajie.cn

[D02] 追加元素到末尾
来源：http://aj.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xk.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hv.521024.cn

JS:   arr.push(4);
来源：http://du.shtwfgs.cn

TS:   arr.push(4);
来源：http://wr.gzmigu.cn

Java: list.add(4);
来源：http://dh.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://wq.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://zn.huixiangedu.cn

C#:   list.Add(4);
来源：http://te.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://fd.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://se.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://td.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ja.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://lk.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://br.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://no.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ww.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://yr.shtwfgs.cn

[D04] 删除元素
来源：http://vu.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zd.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pg.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://he.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://tc.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yg.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://os.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lm.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://em.szsharing.cn

[D05] 访问与修改元素
来源：http://ag.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hg.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rq.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wq.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://uv.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://nx.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ry.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jo.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qk.yuntaijiaju.cn

[D06] 数组长度
来源：http://wc.chemitech.net.cn

Py:   len(arr)
来源：http://pz.9csxet.cn

PHP:  count($arr);
来源：http://yu.shxzukj.cn

JS:   arr.length
来源：http://qe.yuexingan06.cn

TS:   arr.length
来源：http://sw.szsharing.cn

Java: list.size();
来源：http://zw.colortex.cn

Go:   len(arr)
来源：http://hb.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://mx.huixinmuqiang.cn

C#:   list.Count;
来源：http://vc.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://qk.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sb.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sx.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://ka.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://pm.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://ux.asd995.cn

Go:   arr[1:4]
来源：http://xt.shxzukj.cn

Ruby: arr[1, 3]
来源：http://wl.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://bc.szxytkj.cn

[D08] 合并两个数组
来源：http://oq.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://hm.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://gh.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hg.shtwfgs.cn

TS:   [...a, ...b];
来源：http://oa.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iq.asd995.cn

Go:   append(a, b...)
来源：http://mg.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://pl.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://je.huanxung.cn

[D09] 排序（升序）
来源：http://sx.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://eo.bjjhwx.cn

PHP:  sort($arr);
来源：http://cn.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yp.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qo.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jl.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yo.huixiangedu.cn

Ruby: arr.sort
来源：http://ex.bookmarksfly.cn

C#:   list.Sort();
来源：http://da.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ai.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cf.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zf.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kz.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gj.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pu.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hv.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vp.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rx.chemitech.net.cn

[D11] 反转数组
来源：http://kg.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ap.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://qk.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sg.szsharing.cn


<!-- 参考信息 -->