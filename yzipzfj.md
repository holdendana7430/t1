代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fl.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ol.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vv.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fq.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wd.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gx.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://mz.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://ih.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://de.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tp.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gj.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ba.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://nq.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wr.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://gu.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vo.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://th.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nq.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dl.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ud.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cc.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cp.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eq.521024.cn

[B13] 判断是否为数字
来源：http://vn.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://bh.shxzukj.cn

PHP:  is_numeric($x)
来源：http://an.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mo.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://do.asd995.cn

Java: x instanceof Number
来源：http://ll.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vo.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://hh.hahajie.cn

C#:   x is int or double or decimal
来源：http://tj.nszjky.cn

[B14] 判断值是否在集合内
来源：http://sc.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://si.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://io.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ws.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://os.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ll.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dd.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mt.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tt.gzmigu.cn

[B15] 布尔运算与取反
来源：http://qw.9csxet.cn

Py:   a and b or not c
来源：http://ph.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://uy.hahajie.cn

JS:   a && b || !c
来源：http://ke.newstarts.cn

TS:   a && b || !c
来源：http://uh.hahajie.cn

Java: a && b || !c
来源：http://ei.panjiajie.cn

Go:   a && b || !c
来源：http://hi.chemitech.net.cn

Ruby: a && b || !c
来源：http://pi.nszjky.cn

C#:   a && b || !c
来源：http://im.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wr.szsharing.cn

Py:   if not data: return
来源：http://xf.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://fu.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://nn.muxihuayi.cn

TS:   if (!data) return;
来源：http://sm.szxytkj.cn

Java: if (data == null) return;
来源：http://kz.hnjuh.cn

Go:   if data == nil { return }
来源：http://cb.szxytkj.cn

Ruby: return if data.nil?
来源：http://ve.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://zv.huixiangedu.cn

================================================================================
来源：http://my.huixiangedu.cn

C. 函数与作用域
来源：http://hb.yuexingan06.cn

================================================================================
来源：http://bz.yuexingan06.cn

[C01] 定义函数
来源：http://nm.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://zz.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ay.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://eh.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bo.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ds.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jr.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://tw.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ht.nszjky.cn

[C02] 默认参数
来源：http://fe.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://ue.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jv.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://fb.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rm.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xu.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ut.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://sx.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://re.shxzskj.cn

[C03] 可变参数
来源：http://zj.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://qy.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nz.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ew.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kc.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fi.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ic.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://md.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ul.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://uy.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hi.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://el.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://li.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wa.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://yv.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://so.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://ys.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://iz.hahajie.cn

[C05] 返回多个值
来源：http://ob.huixinmuqiang.cn

Py:   return a, b
来源：http://pj.521024.cn

PHP:  return [$a, $b];
来源：http://io.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bf.chemitech.net.cn

TS:   return { a, b };
来源：http://ey.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kb.521024.cn

Go:   return a, b
来源：http://mw.jianghongdianzi.cn

Ruby: return a, b
来源：http://kk.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ol.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://rt.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://po.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://by.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://aj.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ot.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kc.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zf.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://zc.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zz.9csxet.cn

[C07] 把函数作为参数传入
来源：http://hr.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wa.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ch.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lf.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://yk.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ry.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kg.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://gi.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://is.szsharing.cn

[C08] 闭包
来源：http://gq.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xo.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kw.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mk.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ka.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bb.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ze.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nl.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cx.asd995.cn

[C09] 递归
来源：http://ov.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cj.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://au.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nz.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jp.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hv.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ad.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lt.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sg.shxzskj.cn

[C10] 变量作用域
来源：http://wu.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jy.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ej.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hc.szxytkj.cn

TS:   同 JS
来源：http://vm.shxzukj.cn

Java: 方法内为块级作用域
来源：http://hk.jctech888.com.cn

Go:   花括号块级作用域
来源：http://vs.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zp.newstarts.cn

C#:   块级作用域
来源：http://ef.huanxung.cn

[C11] 模块导入与导出
来源：http://yy.huixiangedu.cn

Py:   from module import func
来源：http://gl.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hv.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fh.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cn.lnxyls.cn

Java: import java.util.List;
来源：http://aq.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://os.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://gr.9csxet.cn

C#:   using System.Text;
来源：http://bv.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://we.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://ur.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://ll.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ba.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://bq.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://os.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://vd.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://vy.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://el.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://gu.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nm.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pp.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ke.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pa.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yn.9csxet.cn

Go:   func add(a, b int) int
来源：http://kx.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rd.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jh.yuexingan06.cn

[C14] 泛型函数
来源：http://pp.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://na.wgjwhj.cn

PHP:  // 无泛型
来源：http://vc.shtwfgs.cn

JS:   // 无泛型
来源：http://pb.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ei.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://at.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lz.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://hc.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nq.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://of.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fm.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://tq.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://st.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kq.muxihuayi.cn

Java: // 无解构
来源：http://yz.bjjhwx.cn

Go:   // 无解构
来源：http://tq.gzmigu.cn

Ruby: a, b = pair
来源：http://ys.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://bl.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://mq.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fd.jctech888.com.cn

PHP:  // 无重载
来源：http://uo.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wy.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://bw.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jz.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://tl.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://gy.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qh.haigaiapp.cn

================================================================================
来源：http://bc.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://tt.newstarts.cn

================================================================================
来源：http://na.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://as.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://md.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pn.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ar.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yk.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pd.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://px.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://yb.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jh.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://me.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://or.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vw.nszjky.cn

JS:   arr.push(4);
来源：http://rv.hnjuh.cn

TS:   arr.push(4);
来源：http://qt.szxytkj.cn

Java: list.add(4);
来源：http://bq.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://sh.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://au.9csxet.cn

C#:   list.Add(4);
来源：http://rq.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://es.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://pi.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gf.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vu.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ju.szsharing.cn

Java: list.add(0, 0);
来源：http://yh.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yi.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kv.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ft.hnjuh.cn

[D04] 删除元素
来源：http://ij.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ci.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bw.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fy.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://om.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pr.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://di.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zs.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uz.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://ly.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sn.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uy.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hj.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://cy.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://sh.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://ln.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qo.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hn.yuntaijiaju.cn

[D06] 数组长度
来源：http://ak.huixinmuqiang.cn

Py:   len(arr)
来源：http://ss.bjjhwx.cn

PHP:  count($arr);
来源：http://vo.hnjuh.cn

JS:   arr.length
来源：http://hx.gzmigu.cn

TS:   arr.length
来源：http://lu.9csxet.cn

Java: list.size();
来源：http://hu.nicolike.cn

Go:   len(arr)
来源：http://qp.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://lh.newstarts.cn

C#:   list.Count;
来源：http://jx.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://mj.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vl.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sp.colortex.cn

JS:   arr.slice(1, 4);
来源：http://zs.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://kb.huanxung.cn

Java: list.subList(1, 4);
来源：http://sh.9csxet.cn

Go:   arr[1:4]
来源：http://zz.shxzskj.cn

Ruby: arr[1, 3]
来源：http://bi.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://xm.jctech888.com.cn

[D08] 合并两个数组
来源：http://ng.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://gv.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://yx.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qv.szsharing.cn

TS:   [...a, ...b];
来源：http://wz.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vf.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://qz.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://db.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://ap.521024.cn

[D09] 排序（升序）
来源：http://pb.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://cm.szxytkj.cn

PHP:  sort($arr);
来源：http://zl.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eb.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rq.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vn.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.bjjhwx.cn

Ruby: arr.sort
来源：http://qa.shxzskj.cn

C#:   list.Sort();
来源：http://hw.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yg.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zv.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rz.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cd.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ai.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tz.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qq.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fz.shxzskj.cn


<!-- 参考信息 -->