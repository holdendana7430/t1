代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wn.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://zd.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ep.haigaiapp.cn

[B12] 跳出多层循环
来源：http://bz.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pr.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qg.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://go.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://no.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fh.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zb.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mv.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cu.lnxyls.cn

[B13] 判断是否为数字
来源：http://qw.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://rs.nszjky.cn

PHP:  is_numeric($x)
来源：http://gz.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fs.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pc.huixinmuqiang.cn

Java: x instanceof Number
来源：http://ea.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oj.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://dh.hahajie.cn

C#:   x is int or double or decimal
来源：http://ht.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://vd.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sb.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://pi.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://fj.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ko.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rv.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ra.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cu.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://rb.panjiajie.cn

Py:   a and b or not c
来源：http://yj.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://lu.jctech888.com.cn

JS:   a && b || !c
来源：http://ls.yuexingan06.cn

TS:   a && b || !c
来源：http://qf.huixinmuqiang.cn

Java: a && b || !c
来源：http://pw.shxzskj.cn

Go:   a && b || !c
来源：http://fu.jctech888.com.cn

Ruby: a && b || !c
来源：http://ft.hnjuh.cn

C#:   a && b || !c
来源：http://oj.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fs.szsharing.cn

Py:   if not data: return
来源：http://xn.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://gw.asd995.cn

JS:   if (!data) return;
来源：http://cb.shtwfgs.cn

TS:   if (!data) return;
来源：http://bl.bookmarksfly.cn

Java: if (data == null) return;
来源：http://cz.panjiajie.cn

Go:   if data == nil { return }
来源：http://tt.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://hi.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ie.szsharing.cn

================================================================================
来源：http://nm.huixinmuqiang.cn

C. 函数与作用域
来源：http://up.colortex.cn

================================================================================
来源：http://br.nicolike.cn

[C01] 定义函数
来源：http://ae.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://to.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://he.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://vz.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fn.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fy.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nx.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://pt.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jz.bjjhwx.cn

[C02] 默认参数
来源：http://yl.521024.cn

Py:   def greet(name="World"): return name
来源：http://ts.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://an.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://uv.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cm.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cw.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iz.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://dx.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://so.huixinmuqiang.cn

[C03] 可变参数
来源：http://tm.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://sa.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rv.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://au.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bu.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hf.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://go.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://li.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mp.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://yh.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jx.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fv.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vd.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wl.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ir.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://iy.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://ii.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://og.jianghongdianzi.cn

[C05] 返回多个值
来源：http://xp.nicolike.cn

Py:   return a, b
来源：http://lu.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ig.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ew.hahajie.cn

TS:   return { a, b };
来源：http://bs.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zb.lnxyls.cn

Go:   return a, b
来源：http://dv.nicolike.cn

Ruby: return a, b
来源：http://uz.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://rp.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://gy.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://ra.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yp.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://fj.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://co.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bd.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vv.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://jr.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ho.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://ma.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vb.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zk.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fw.hahajie.cn

TS:   arr.map(String)
来源：http://jg.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aq.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mk.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://zq.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lm.chemitech.net.cn

[C08] 闭包
来源：http://qq.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wh.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ck.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uf.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ly.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vw.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mp.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dc.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ad.shtwfgs.cn

[C09] 递归
来源：http://vb.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jj.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wf.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iv.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://os.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jv.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kg.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yx.chemitech.net.cn

[C10] 变量作用域
来源：http://bd.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cr.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ct.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bu.chemitech.net.cn

TS:   同 JS
来源：http://vm.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://wh.nszjky.cn

Go:   花括号块级作用域
来源：http://bs.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nu.huanxung.cn

C#:   块级作用域
来源：http://ge.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ci.jctech888.com.cn

Py:   from module import func
来源：http://sx.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cb.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ht.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ta.lnxyls.cn

Java: import java.util.List;
来源：http://oz.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ub.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://un.newstarts.cn

C#:   using System.Text;
来源：http://oo.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://au.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://uu.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://pu.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://uw.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://bh.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tf.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://lm.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://co.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fi.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://de.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tq.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lg.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nz.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mk.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cy.szxytkj.cn

Go:   func add(a, b int) int
来源：http://jf.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://em.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gp.colortex.cn

[C14] 泛型函数
来源：http://tj.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bp.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://rs.huixiangedu.cn

JS:   // 无泛型
来源：http://gu.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cv.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ek.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uw.hahajie.cn

Ruby: # 无泛型
来源：http://my.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://av.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://sa.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gh.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://si.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uy.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dt.hahajie.cn

Java: // 无解构
来源：http://kx.colortex.cn

Go:   // 无解构
来源：http://lx.huanxung.cn

Ruby: a, b = pair
来源：http://ek.huanxung.cn

C#:   var (a, b) = pair;
来源：http://et.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://cx.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qa.hnjuh.cn

PHP:  // 无重载
来源：http://fe.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://th.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://mn.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ar.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://pb.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://ou.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vb.bookmarksfly.cn

================================================================================
来源：http://lh.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://jx.szsharing.cn

================================================================================
来源：http://id.colortex.cn

[D01] 创建数组 / 列表
来源：http://mt.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://py.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bx.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ac.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ep.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://br.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://iz.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://ch.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ez.asd995.cn

[D02] 追加元素到末尾
来源：http://mf.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ev.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pb.huanxung.cn

JS:   arr.push(4);
来源：http://cb.shxzukj.cn

TS:   arr.push(4);
来源：http://pc.nicolike.cn

Java: list.add(4);
来源：http://dx.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://hd.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ev.shtwfgs.cn

C#:   list.Add(4);
来源：http://ub.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://ao.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://cr.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://os.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ql.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ys.chemitech.net.cn

Java: list.add(0, 0);
来源：http://sh.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aq.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cu.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://zp.huanxung.cn

[D04] 删除元素
来源：http://ja.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ol.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://is.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ns.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://de.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cd.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://es.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ke.colortex.cn

[D05] 访问与修改元素
来源：http://wy.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hp.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ml.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ld.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://mk.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://pz.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://dd.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nf.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fo.asd995.cn

[D06] 数组长度
来源：http://bs.huixiangedu.cn

Py:   len(arr)
来源：http://sk.jianghongdianzi.cn

PHP:  count($arr);
来源：http://sp.huixiangedu.cn

JS:   arr.length
来源：http://oj.lnxyls.cn

TS:   arr.length
来源：http://xm.bjjhwx.cn

Java: list.size();
来源：http://aa.huanxung.cn

Go:   len(arr)
来源：http://bz.521024.cn

Ruby: arr.length; arr.size
来源：http://ub.wgjwhj.cn

C#:   list.Count;
来源：http://li.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://wr.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zl.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ox.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://ie.asd995.cn

TS:   arr.slice(1, 4);
来源：http://pd.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://in.nszjky.cn

Go:   arr[1:4]
来源：http://sv.gzmigu.cn

Ruby: arr[1, 3]
来源：http://qy.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://kh.newstarts.cn

[D08] 合并两个数组
来源：http://fp.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://pj.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://cq.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ax.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://me.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ms.huanxung.cn

Go:   append(a, b...)
来源：http://fu.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://tx.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://qv.haigaiapp.cn

[D09] 排序（升序）
来源：http://tk.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fy.bjjhwx.cn

PHP:  sort($arr);
来源：http://uy.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dz.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hc.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cx.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ps.huixiangedu.cn

Ruby: arr.sort
来源：http://zf.hahajie.cn

C#:   list.Sort();
来源：http://ut.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mz.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uy.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ci.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dy.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dw.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ml.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ix.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mk.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ua.panjiajie.cn

[D11] 反转数组
来源：http://xn.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pr.huanxung.cn

PHP:  array_reverse($arr);
来源：http://fd.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://un.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://bf.huanxung.cn

Java: Collections.reverse(list);
来源：http://lj.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://sn.shxzskj.cn

Ruby: arr.reverse
来源：http://dg.shxzukj.cn

C#:   list.Reverse();
来源：http://tr.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://uk.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://lm.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tj.muxihuayi.cn


<!-- 参考信息 -->