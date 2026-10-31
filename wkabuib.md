代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ya.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ki.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://em.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://dx.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ql.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ky.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dg.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pz.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ym.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://se.hnjuh.cn

[B12] 跳出多层循环
来源：http://me.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wg.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kn.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ws.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yy.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ng.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ni.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lg.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hq.nicolike.cn

[B13] 判断是否为数字
来源：http://ju.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://zr.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://hr.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rp.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fi.hnjuh.cn

Java: x instanceof Number
来源：http://hx.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hm.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://uh.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://kp.newstarts.cn

[B14] 判断值是否在集合内
来源：http://um.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fz.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://di.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://rt.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://qz.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gr.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lt.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bp.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wv.9csxet.cn

[B15] 布尔运算与取反
来源：http://bg.haigaiapp.cn

Py:   a and b or not c
来源：http://un.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://te.jianghongdianzi.cn

JS:   a && b || !c
来源：http://qo.huanxung.cn

TS:   a && b || !c
来源：http://ji.9csxet.cn

Java: a && b || !c
来源：http://vi.chemitech.net.cn

Go:   a && b || !c
来源：http://oo.shxzukj.cn

Ruby: a && b || !c
来源：http://cb.9csxet.cn

C#:   a && b || !c
来源：http://fg.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rb.muxihuayi.cn

Py:   if not data: return
来源：http://mo.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://hc.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://fw.asd995.cn

TS:   if (!data) return;
来源：http://qw.szxytkj.cn

Java: if (data == null) return;
来源：http://tg.jctech888.com.cn

Go:   if data == nil { return }
来源：http://fs.shtwfgs.cn

Ruby: return if data.nil?
来源：http://wt.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ik.haigaiapp.cn

================================================================================
来源：http://te.huixiangedu.cn

C. 函数与作用域
来源：http://fj.chemitech.net.cn

================================================================================
来源：http://fb.shxzskj.cn

[C01] 定义函数
来源：http://gw.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://hs.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dr.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://eu.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qb.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wv.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ue.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://nv.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ce.muxihuayi.cn

[C02] 默认参数
来源：http://ff.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://el.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://io.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://eq.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vm.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ma.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xy.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://li.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://iy.muxihuayi.cn

[C03] 可变参数
来源：http://tp.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ey.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ww.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rj.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sk.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wh.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bp.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qr.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lf.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ao.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jp.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eu.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ju.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hj.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ta.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://es.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://dt.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://xu.9csxet.cn

[C05] 返回多个值
来源：http://rj.yuexingan06.cn

Py:   return a, b
来源：http://vz.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ke.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fo.nicolike.cn

TS:   return { a, b };
来源：http://no.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ed.wgjwhj.cn

Go:   return a, b
来源：http://oj.muxihuayi.cn

Ruby: return a, b
来源：http://nu.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://yb.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://er.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://jo.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iw.shxzukj.cn

JS:   const square = x => x * x;
来源：http://bo.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://oe.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ks.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pv.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://lm.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vt.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://pc.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ul.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gh.szsharing.cn

TS:   arr.map(String)
来源：http://lj.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lo.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ew.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://oa.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sh.bjjhwx.cn

[C08] 闭包
来源：http://wp.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lp.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wh.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iw.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bd.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tz.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tq.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://py.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://or.huixinmuqiang.cn

[C09] 递归
来源：http://ev.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kk.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rb.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bt.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xq.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ay.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dt.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://af.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gm.huixiangedu.cn

[C10] 变量作用域
来源：http://wf.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://el.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cv.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lb.bjjhwx.cn

TS:   同 JS
来源：http://oj.gzmigu.cn

Java: 方法内为块级作用域
来源：http://zu.newstarts.cn

Go:   花括号块级作用域
来源：http://wn.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.shxzukj.cn

C#:   块级作用域
来源：http://jo.gzmigu.cn

[C11] 模块导入与导出
来源：http://mw.yuntaijiaju.cn

Py:   from module import func
来源：http://oc.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yk.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qi.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://my.nszjky.cn

Java: import java.util.List;
来源：http://km.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wn.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://ay.colortex.cn

C#:   using System.Text;
来源：http://rt.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://sk.asd995.cn

Py:   (lambda: print("run"))()
来源：http://jb.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://xi.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ti.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://je.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yx.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://wz.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://oj.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bm.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://hj.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fa.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zi.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xb.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wq.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wj.hnjuh.cn

Go:   func add(a, b int) int
来源：http://jk.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ki.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oy.yuntaijiaju.cn

[C14] 泛型函数
来源：http://de.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hl.bjjhwx.cn

PHP:  // 无泛型
来源：http://sj.bjjhwx.cn

JS:   // 无泛型
来源：http://xf.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dj.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://of.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lb.muxihuayi.cn

Ruby: # 无泛型
来源：http://nn.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wi.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://dn.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yv.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://ct.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kh.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ex.hahajie.cn

Java: // 无解构
来源：http://qr.szxytkj.cn

Go:   // 无解构
来源：http://ox.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://wk.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://hg.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://hb.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://td.newstarts.cn

PHP:  // 无重载
来源：http://vo.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xj.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://qa.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zx.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ne.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://md.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ba.yuntaijiaju.cn

================================================================================
来源：http://rh.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://vo.chemitech.net.cn

================================================================================
来源：http://pz.hahajie.cn

[D01] 创建数组 / 列表
来源：http://bv.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ks.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ct.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tw.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qx.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ne.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://sv.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://mm.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fb.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://hw.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xm.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wi.hnjuh.cn

JS:   arr.push(4);
来源：http://qy.shxzukj.cn

TS:   arr.push(4);
来源：http://er.huixinmuqiang.cn

Java: list.add(4);
来源：http://az.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ax.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://rc.hahajie.cn

C#:   list.Add(4);
来源：http://bi.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://kn.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://hx.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kt.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bb.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://uv.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://ur.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vp.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cu.521024.cn

C#:   list.Insert(0, 0);
来源：http://nx.wgjwhj.cn

[D04] 删除元素
来源：http://fe.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hk.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hp.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jm.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://mw.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tc.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ln.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sf.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dx.hnjuh.cn

[D05] 访问与修改元素
来源：http://wo.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://da.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xy.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sg.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://pq.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://tb.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://lb.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kt.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hq.shxzskj.cn

[D06] 数组长度
来源：http://cv.wgjwhj.cn

Py:   len(arr)
来源：http://mm.colortex.cn

PHP:  count($arr);
来源：http://cr.huixinmuqiang.cn

JS:   arr.length
来源：http://ib.szsharing.cn

TS:   arr.length
来源：http://zw.wgjwhj.cn

Java: list.size();
来源：http://kp.yuntaijiaju.cn

Go:   len(arr)
来源：http://wj.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://bu.hahajie.cn

C#:   list.Count;
来源：http://kc.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://xq.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gx.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gp.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://gx.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://dz.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://vt.asd995.cn

Go:   arr[1:4]
来源：http://kk.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://jj.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://cs.colortex.cn

[D08] 合并两个数组
来源：http://do.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://pz.colortex.cn

PHP:  array_merge($a, $b);
来源：http://bg.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dm.nszjky.cn

TS:   [...a, ...b];
来源：http://ie.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ds.asd995.cn

Go:   append(a, b...)
来源：http://sv.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://fl.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://uh.shxzskj.cn

[D09] 排序（升序）
来源：http://nk.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://di.bjjhwx.cn

PHP:  sort($arr);
来源：http://cv.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zs.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ou.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yp.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://if.colortex.cn

Ruby: arr.sort
来源：http://sw.szsharing.cn

C#:   list.Sort();
来源：http://pw.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xs.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vq.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oo.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ap.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ej.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kg.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xm.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lf.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wu.asd995.cn

[D11] 反转数组
来源：http://yk.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hi.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://bm.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dz.jctech888.com.cn


<!-- 参考信息 -->