代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://xs.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zh.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rz.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://en.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ca.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ie.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wk.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://fh.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://sn.szxytkj.cn

PHP:  is_numeric($x)
来源：http://if.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lp.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://im.shtwfgs.cn

Java: x instanceof Number
来源：http://kn.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oh.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://uu.szsharing.cn

C#:   x is int or double or decimal
来源：http://gj.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://sw.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wf.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kw.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://bx.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://fd.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ii.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kd.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rd.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gu.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://af.szsharing.cn

Py:   a and b or not c
来源：http://zq.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://te.huanxung.cn

JS:   a && b || !c
来源：http://az.shxzukj.cn

TS:   a && b || !c
来源：http://ct.shxzskj.cn

Java: a && b || !c
来源：http://pw.nszjky.cn

Go:   a && b || !c
来源：http://sw.shtwfgs.cn

Ruby: a && b || !c
来源：http://jm.yuntaijiaju.cn

C#:   a && b || !c
来源：http://yo.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pj.shxzukj.cn

Py:   if not data: return
来源：http://yy.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://nl.hnjuh.cn

JS:   if (!data) return;
来源：http://ad.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://vk.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://rf.chemitech.net.cn

Go:   if data == nil { return }
来源：http://qn.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://bk.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://pw.jianghongdianzi.cn

================================================================================
来源：http://wq.nszjky.cn

C. 函数与作用域
来源：http://wk.colortex.cn

================================================================================
来源：http://cu.bookmarksfly.cn

[C01] 定义函数
来源：http://oj.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://ip.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://tf.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iv.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pu.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://in.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://jz.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oo.newstarts.cn

[C02] 默认参数
来源：http://pr.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://sl.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wi.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://ke.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rs.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://df.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://wp.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://jc.gzmigu.cn

[C03] 可变参数
来源：http://yp.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://yy.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mm.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cy.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fv.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ua.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uj.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oq.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://tv.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uv.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ty.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uv.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zm.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://re.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://uk.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://tv.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://qf.gzmigu.cn

[C05] 返回多个值
来源：http://yd.521024.cn

Py:   return a, b
来源：http://ov.hnjuh.cn

PHP:  return [$a, $b];
来源：http://ti.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zo.szxytkj.cn

TS:   return { a, b };
来源：http://ek.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nx.hnjuh.cn

Go:   return a, b
来源：http://eo.huixiangedu.cn

Ruby: return a, b
来源：http://rk.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ys.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://hs.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ab.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://al.gzmigu.cn

JS:   const square = x => x * x;
来源：http://xb.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://sq.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hg.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aj.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://pw.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zi.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://hf.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ae.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nc.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rm.huanxung.cn

TS:   arr.map(String)
来源：http://ah.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bg.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rw.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://vi.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ra.wgjwhj.cn

[C08] 闭包
来源：http://br.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gz.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qx.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rq.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ni.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hd.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xg.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ac.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yp.huixinmuqiang.cn

[C09] 递归
来源：http://jo.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oc.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rb.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wf.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dz.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nn.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kc.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xr.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tq.huixinmuqiang.cn

[C10] 变量作用域
来源：http://bq.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zg.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sf.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oc.newstarts.cn

TS:   同 JS
来源：http://ws.9csxet.cn

Java: 方法内为块级作用域
来源：http://jz.gzmigu.cn

Go:   花括号块级作用域
来源：http://yv.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ou.shxzukj.cn

C#:   块级作用域
来源：http://rb.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://yw.yuntaijiaju.cn

Py:   from module import func
来源：http://os.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nj.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xk.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bj.huanxung.cn

Java: import java.util.List;
来源：http://tm.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tt.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ek.panjiajie.cn

C#:   using System.Text;
来源：http://qv.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://vy.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://es.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://in.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://zo.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://nf.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cj.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://cs.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://vc.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ct.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://oe.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vp.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jh.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fk.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ly.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ra.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://ut.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ra.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gn.bjjhwx.cn

[C14] 泛型函数
来源：http://xz.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xx.hnjuh.cn

PHP:  // 无泛型
来源：http://cp.521024.cn

JS:   // 无泛型
来源：http://zx.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bo.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cr.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kk.hahajie.cn

Ruby: # 无泛型
来源：http://wo.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ow.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://qt.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yx.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://zt.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lw.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wi.newstarts.cn

Java: // 无解构
来源：http://zt.521024.cn

Go:   // 无解构
来源：http://ir.panjiajie.cn

Ruby: a, b = pair
来源：http://og.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://gw.huanxung.cn

[C16] 函数 / 方法重载
来源：http://qe.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zg.haigaiapp.cn

PHP:  // 无重载
来源：http://qr.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qw.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://mw.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dt.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://cv.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ll.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vw.gzmigu.cn

================================================================================
来源：http://qf.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://jq.huixiangedu.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://zc.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oy.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pi.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://so.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nn.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fs.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://uu.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://ew.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aa.szxytkj.cn

[D02] 追加元素到末尾
来源：http://ku.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gn.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fl.chemitech.net.cn

JS:   arr.push(4);
来源：http://iq.shtwfgs.cn

TS:   arr.push(4);
来源：http://au.shxzskj.cn

Java: list.add(4);
来源：http://bd.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://ad.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://fm.wgjwhj.cn

C#:   list.Add(4);
来源：http://hk.nszjky.cn

[D03] 在指定位置插入元素
来源：http://jl.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://sw.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ix.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ov.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://yt.521024.cn

Java: list.add(0, 0);
来源：http://hm.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oc.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gk.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ga.shxzskj.cn

[D04] 删除元素
来源：http://bx.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mk.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gk.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bx.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://eb.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jp.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ek.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://la.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gw.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://rh.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ei.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oi.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oo.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://jr.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://gf.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://bh.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zw.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dl.huanxung.cn

[D06] 数组长度
来源：http://tf.asd995.cn

Py:   len(arr)
来源：http://wd.yuntaijiaju.cn

PHP:  count($arr);
来源：http://nl.nszjky.cn

JS:   arr.length
来源：http://ml.wgjwhj.cn

TS:   arr.length
来源：http://ch.jctech888.com.cn

Java: list.size();
来源：http://wr.bjjhwx.cn

Go:   len(arr)
来源：http://wb.521024.cn

Ruby: arr.length; arr.size
来源：http://or.nszjky.cn

C#:   list.Count;
来源：http://oz.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://uw.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jt.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xb.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://th.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://nq.szsharing.cn

Java: list.subList(1, 4);
来源：http://ye.hnjuh.cn

Go:   arr[1:4]
来源：http://md.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://kt.521024.cn

C#:   list.GetRange(1, 3);
来源：http://np.521024.cn

[D08] 合并两个数组
来源：http://ob.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://mj.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://ub.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://op.wgjwhj.cn

TS:   [...a, ...b];
来源：http://ra.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vo.newstarts.cn

Go:   append(a, b...)
来源：http://rj.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://dj.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://eq.szxytkj.cn

[D09] 排序（升序）
来源：http://ao.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.panjiajie.cn

PHP:  sort($arr);
来源：http://wu.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ab.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xq.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yo.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wr.shxzukj.cn

Ruby: arr.sort
来源：http://uu.hahajie.cn

C#:   list.Sort();
来源：http://px.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yd.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ig.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bi.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pl.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rl.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nh.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ls.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yt.chemitech.net.cn

[D11] 反转数组
来源：http://cv.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ez.nszjky.cn

PHP:  array_reverse($arr);
来源：http://vr.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://af.panjiajie.cn

TS:   [...arr].reverse();
来源：http://ln.9csxet.cn

Java: Collections.reverse(list);
来源：http://zk.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://gx.gzmigu.cn

Ruby: arr.reverse
来源：http://yy.hahajie.cn

C#:   list.Reverse();
来源：http://mk.gzmigu.cn

[D12] 查找元素下标
来源：http://jp.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://ly.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pc.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ss.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://of.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://gh.yuexingan06.cn


<!-- 参考信息 -->