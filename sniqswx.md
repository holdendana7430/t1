代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.newstarts.cn

[B10] 遍历同时拿索引
来源：http://ow.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hf.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://br.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lc.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jc.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ze.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xa.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vk.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ya.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ng.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://ah.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ju.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zl.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pl.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pb.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ni.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dm.nszjky.cn

[B12] 跳出多层循环
来源：http://vq.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xl.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qq.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yp.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cl.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bd.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ln.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lp.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tj.lnxyls.cn

[B13] 判断是否为数字
来源：http://hq.521024.cn

Py:   isinstance(x, (int, float))
来源：http://kq.hahajie.cn

PHP:  is_numeric($x)
来源：http://gl.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://it.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xw.bookmarksfly.cn

Java: x instanceof Number
来源：http://bw.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sr.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://if.newstarts.cn

C#:   x is int or double or decimal
来源：http://jo.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://hb.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hs.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ry.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://to.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ov.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tv.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vo.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cc.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dn.lnxyls.cn

[B15] 布尔运算与取反
来源：http://no.yuexingan06.cn

Py:   a and b or not c
来源：http://zk.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://fl.nszjky.cn

JS:   a && b || !c
来源：http://ba.huixiangedu.cn

TS:   a && b || !c
来源：http://ma.szsharing.cn

Java: a && b || !c
来源：http://tj.yuntaijiaju.cn

Go:   a && b || !c
来源：http://bk.panjiajie.cn

Ruby: a && b || !c
来源：http://gm.yuexingan06.cn

C#:   a && b || !c
来源：http://fo.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tz.szsharing.cn

Py:   if not data: return
来源：http://lm.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://kq.chemitech.net.cn

JS:   if (!data) return;
来源：http://mk.huixiangedu.cn

TS:   if (!data) return;
来源：http://rl.hahajie.cn

Java: if (data == null) return;
来源：http://jy.hahajie.cn

Go:   if data == nil { return }
来源：http://lz.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://vf.colortex.cn

C#:   if (data == null) return;
来源：http://cz.szxytkj.cn

================================================================================
来源：http://gx.newstarts.cn

C. 函数与作用域
来源：http://ql.hnjuh.cn

================================================================================
来源：http://ug.huixinmuqiang.cn

[C01] 定义函数
来源：http://bj.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://wj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ib.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://ji.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tc.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uj.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sy.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ve.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vk.hnjuh.cn

[C02] 默认参数
来源：http://fz.colortex.cn

Py:   def greet(name="World"): return name
来源：http://fn.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sj.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://gb.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://af.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nc.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ka.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://lx.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://xt.panjiajie.cn

[C03] 可变参数
来源：http://ap.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://ku.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ss.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vs.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dm.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vs.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ha.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oy.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ry.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://kh.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gm.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ue.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dn.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sr.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://pe.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://we.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://pb.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://sl.jianghongdianzi.cn

[C05] 返回多个值
来源：http://qu.9csxet.cn

Py:   return a, b
来源：http://tk.hnjuh.cn

PHP:  return [$a, $b];
来源：http://cp.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yl.nszjky.cn

TS:   return { a, b };
来源：http://sq.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jh.hnjuh.cn

Go:   return a, b
来源：http://bk.panjiajie.cn

Ruby: return a, b
来源：http://ch.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ye.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://uf.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://yl.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pt.newstarts.cn

JS:   const square = x => x * x;
来源：http://yt.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://uh.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fc.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zl.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://wh.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yx.521024.cn

[C07] 把函数作为参数传入
来源：http://xk.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ur.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tm.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yy.bookmarksfly.cn

TS:   arr.map(String)
来源：http://kd.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jr.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vf.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://sv.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ja.newstarts.cn

[C08] 闭包
来源：http://bj.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yt.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ct.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xy.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://af.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qd.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fd.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wb.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zu.jctech888.com.cn

[C09] 递归
来源：http://oy.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sr.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eg.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dd.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qw.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zg.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zx.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jx.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ok.bjjhwx.cn

[C10] 变量作用域
来源：http://dc.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ba.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ir.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://as.yuntaijiaju.cn

TS:   同 JS
来源：http://lo.szsharing.cn

Java: 方法内为块级作用域
来源：http://ws.shxzukj.cn

Go:   花括号块级作用域
来源：http://uv.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zc.521024.cn

C#:   块级作用域
来源：http://li.szsharing.cn

[C11] 模块导入与导出
来源：http://oj.hahajie.cn

Py:   from module import func
来源：http://ae.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rk.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gq.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pi.hahajie.cn

Java: import java.util.List;
来源：http://je.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ce.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://em.huanxung.cn

C#:   using System.Text;
来源：http://qw.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://kq.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://qj.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://bh.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://rb.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://zk.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jc.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://hw.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://fp.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://as.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://mu.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ni.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://or.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hi.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xm.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gn.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://rt.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dh.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ud.shxzskj.cn

[C14] 泛型函数
来源：http://du.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vk.huanxung.cn

PHP:  // 无泛型
来源：http://jf.muxihuayi.cn

JS:   // 无泛型
来源：http://rw.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qw.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fq.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oe.9csxet.cn

Ruby: # 无泛型
来源：http://ja.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nv.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://mp.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gs.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://wm.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qh.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://py.shtwfgs.cn

Java: // 无解构
来源：http://xs.bjjhwx.cn

Go:   // 无解构
来源：http://kr.szxytkj.cn

Ruby: a, b = pair
来源：http://wc.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://if.szsharing.cn

[C16] 函数 / 方法重载
来源：http://yr.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ch.yuexingan06.cn

PHP:  // 无重载
来源：http://ya.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zg.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ik.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tn.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://nz.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://np.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hc.nicolike.cn

================================================================================
来源：http://hf.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://xr.szxytkj.cn

================================================================================
来源：http://hk.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://zt.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ya.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dc.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ho.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ui.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gl.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://yv.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://wk.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ah.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://zm.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gn.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hy.szxytkj.cn

JS:   arr.push(4);
来源：http://ql.9csxet.cn

TS:   arr.push(4);
来源：http://gv.jianghongdianzi.cn

Java: list.add(4);
来源：http://zg.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://rf.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ps.shtwfgs.cn

C#:   list.Add(4);
来源：http://nr.9csxet.cn

[D03] 在指定位置插入元素
来源：http://wj.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://ad.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wx.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yg.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://fr.9csxet.cn

Java: list.add(0, 0);
来源：http://po.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ux.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nb.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://cm.jctech888.com.cn

[D04] 删除元素
来源：http://do.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jj.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rx.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yc.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://bs.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bn.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jl.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sd.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cc.wgjwhj.cn

[D05] 访问与修改元素
来源：http://vx.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ns.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mp.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ej.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://fr.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://sh.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vt.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hv.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ro.lnxyls.cn

[D06] 数组长度
来源：http://wn.huixiangedu.cn

Py:   len(arr)
来源：http://og.huixiangedu.cn

PHP:  count($arr);
来源：http://uy.hnjuh.cn

JS:   arr.length
来源：http://qa.bookmarksfly.cn

TS:   arr.length
来源：http://mc.panjiajie.cn

Java: list.size();
来源：http://ps.jctech888.com.cn

Go:   len(arr)
来源：http://bg.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://ls.szxytkj.cn

C#:   list.Count;
来源：http://ks.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://ob.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ci.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uk.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ya.colortex.cn

TS:   arr.slice(1, 4);
来源：http://sz.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://qp.nszjky.cn

Go:   arr[1:4]
来源：http://dh.asd995.cn

Ruby: arr[1, 3]
来源：http://mj.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://lu.nszjky.cn

[D08] 合并两个数组
来源：http://gb.521024.cn

Py:   a + b;  a.extend(b)
来源：http://pj.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://rw.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wl.521024.cn

TS:   [...a, ...b];
来源：http://gn.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lz.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://gs.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://sx.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://zv.bjjhwx.cn

[D09] 排序（升序）
来源：http://bh.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://cv.bookmarksfly.cn

PHP:  sort($arr);
来源：http://tx.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ht.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xw.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vy.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jl.hnjuh.cn

Ruby: arr.sort
来源：http://du.yuexingan06.cn

C#:   list.Sort();
来源：http://zk.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hb.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xv.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fn.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lz.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wi.9csxet.cn


<!-- 参考信息 -->