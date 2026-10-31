代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nn.nicolike.cn

[B10] 遍历同时拿索引
来源：http://rv.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bj.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://je.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fh.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://du.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ad.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qd.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jw.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://af.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://so.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://by.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://tp.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ro.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yw.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wm.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jv.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jj.muxihuayi.cn

[B12] 跳出多层循环
来源：http://ov.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fz.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pv.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cg.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://az.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nn.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ed.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ct.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://ar.szxytkj.cn

PHP:  is_numeric($x)
来源：http://aa.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ed.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rq.haigaiapp.cn

Java: x instanceof Number
来源：http://sd.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://io.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://zp.huanxung.cn

C#:   x is int or double or decimal
来源：http://nm.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://kq.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://am.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://lt.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://cg.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://og.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rd.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hw.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ii.lnxyls.cn

[B15] 布尔运算与取反
来源：http://kw.panjiajie.cn

Py:   a and b or not c
来源：http://qg.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://yi.jianghongdianzi.cn

JS:   a && b || !c
来源：http://jx.nicolike.cn

TS:   a && b || !c
来源：http://yj.521024.cn

Java: a && b || !c
来源：http://tm.asd995.cn

Go:   a && b || !c
来源：http://wz.wgjwhj.cn

Ruby: a && b || !c
来源：http://yd.asd995.cn

C#:   a && b || !c
来源：http://ha.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bv.nszjky.cn

Py:   if not data: return
来源：http://qc.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://hz.chemitech.net.cn

JS:   if (!data) return;
来源：http://tk.yuexingan06.cn

TS:   if (!data) return;
来源：http://nf.colortex.cn

Java: if (data == null) return;
来源：http://tp.chemitech.net.cn

Go:   if data == nil { return }
来源：http://cu.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://bs.hahajie.cn

C#:   if (data == null) return;
来源：http://jx.yuexingan06.cn

================================================================================
来源：http://nr.newstarts.cn

C. 函数与作用域
来源：http://et.panjiajie.cn

================================================================================
来源：http://bn.panjiajie.cn

[C01] 定义函数
来源：http://ma.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://be.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tm.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://af.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ni.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://te.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sv.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://zl.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ff.nszjky.cn

[C02] 默认参数
来源：http://zo.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://fm.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ro.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://dq.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wh.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jc.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zv.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://pe.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://gh.nszjky.cn

[C03] 可变参数
来源：http://yv.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://ej.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iq.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jw.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ts.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ss.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mj.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yk.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uk.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://lp.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ay.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zx.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wa.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dp.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://ut.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://wi.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://xi.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://mv.hnjuh.cn

[C05] 返回多个值
来源：http://nt.yuexingan06.cn

Py:   return a, b
来源：http://xb.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://qq.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hp.521024.cn

TS:   return { a, b };
来源：http://yo.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cg.nszjky.cn

Go:   return a, b
来源：http://xc.haigaiapp.cn

Ruby: return a, b
来源：http://nr.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://hg.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://nc.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://tw.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rj.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ml.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ff.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cm.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vk.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://kt.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vl.newstarts.cn

[C07] 把函数作为参数传入
来源：http://hw.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://be.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ic.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vo.jctech888.com.cn

TS:   arr.map(String)
来源：http://yq.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kc.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qy.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://df.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zt.hahajie.cn

[C08] 闭包
来源：http://gu.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yr.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://as.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cq.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://px.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ej.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vi.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zf.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tu.lnxyls.cn

[C09] 递归
来源：http://lk.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fx.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hm.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qf.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://il.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gb.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nj.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lg.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sv.wgjwhj.cn

[C10] 变量作用域
来源：http://gb.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vu.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ym.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cw.yuntaijiaju.cn

TS:   同 JS
来源：http://qf.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://hz.chemitech.net.cn

Go:   花括号块级作用域
来源：http://ig.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xt.yuntaijiaju.cn

C#:   块级作用域
来源：http://zi.newstarts.cn

[C11] 模块导入与导出
来源：http://oo.gzmigu.cn

Py:   from module import func
来源：http://kg.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ns.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wo.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zd.shtwfgs.cn

Java: import java.util.List;
来源：http://mj.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bm.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://rs.szsharing.cn

C#:   using System.Text;
来源：http://cp.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://us.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://hw.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://ku.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://fw.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://jr.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://em.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ek.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ff.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lk.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://nn.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ah.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mg.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dx.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uj.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.shxzukj.cn

Go:   func add(a, b int) int
来源：http://xm.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xk.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bf.nicolike.cn

[C14] 泛型函数
来源：http://oz.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zy.lnxyls.cn

PHP:  // 无泛型
来源：http://xx.panjiajie.cn

JS:   // 无泛型
来源：http://ks.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eg.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bq.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vw.szxytkj.cn

Ruby: # 无泛型
来源：http://ty.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mn.nicolike.cn

[C15] 解构 / 展开参数
来源：http://ft.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mq.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://og.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yu.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zr.newstarts.cn

Java: // 无解构
来源：http://qq.yuntaijiaju.cn

Go:   // 无解构
来源：http://ay.panjiajie.cn

Ruby: a, b = pair
来源：http://ta.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://ra.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://fh.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://np.szxytkj.cn

PHP:  // 无重载
来源：http://ls.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qf.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ip.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cl.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://fv.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://re.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ry.bookmarksfly.cn

================================================================================
来源：http://zc.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://cd.panjiajie.cn

================================================================================
来源：http://vq.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://fj.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ll.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ga.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xq.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ed.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://we.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://fm.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://hg.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wx.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://dv.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ti.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pm.chemitech.net.cn

JS:   arr.push(4);
来源：http://lm.colortex.cn

TS:   arr.push(4);
来源：http://di.huixinmuqiang.cn

Java: list.add(4);
来源：http://ft.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://hr.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://bd.panjiajie.cn

C#:   list.Add(4);
来源：http://tv.huanxung.cn

[D03] 在指定位置插入元素
来源：http://hv.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://bw.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ta.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hr.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://av.nicolike.cn

Java: list.add(0, 0);
来源：http://zm.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ch.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rk.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ta.shxzskj.cn

[D04] 删除元素
来源：http://gc.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://om.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vd.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bj.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://vh.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sj.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ul.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kt.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vi.bjjhwx.cn

[D05] 访问与修改元素
来源：http://wl.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ky.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pg.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dw.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://wo.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bc.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://hg.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rh.bjjhwx.cn

[D06] 数组长度
来源：http://kg.hahajie.cn

Py:   len(arr)
来源：http://dr.szxytkj.cn

PHP:  count($arr);
来源：http://tv.9csxet.cn

JS:   arr.length
来源：http://mg.nicolike.cn

TS:   arr.length
来源：http://xl.huixinmuqiang.cn

Java: list.size();
来源：http://qw.huanxung.cn

Go:   len(arr)
来源：http://zo.hahajie.cn

Ruby: arr.length; arr.size
来源：http://fz.bjjhwx.cn

C#:   list.Count;
来源：http://mi.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://oj.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xj.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xu.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://jd.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://fs.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://pn.hahajie.cn

Go:   arr[1:4]
来源：http://pp.colortex.cn

Ruby: arr[1, 3]
来源：http://zf.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://hj.shxzskj.cn

[D08] 合并两个数组
来源：http://nf.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://de.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://hx.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uk.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://gu.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eb.huixiangedu.cn

Go:   append(a, b...)
来源：http://xf.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://dd.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://yv.szsharing.cn

[D09] 排序（升序）
来源：http://gz.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://jn.shtwfgs.cn

PHP:  sort($arr);
来源：http://lw.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fz.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ob.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vg.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bz.yuexingan06.cn

Ruby: arr.sort
来源：http://wk.9csxet.cn

C#:   list.Sort();
来源：http://sl.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ks.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eo.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fl.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uz.szxytkj.cn


<!-- 参考信息 -->