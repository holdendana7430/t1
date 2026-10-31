代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ue.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iq.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kt.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bf.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oq.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gl.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nq.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ep.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ma.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://za.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://wn.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://mh.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xk.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zq.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rk.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bz.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://ss.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zv.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://hn.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bt.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://op.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qn.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tv.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gr.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ef.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://an.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vk.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ls.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://dn.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://tv.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cn.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xl.yuntaijiaju.cn

Java: x instanceof Number
来源：http://ik.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kw.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://zi.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://js.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://ua.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ms.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wu.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ha.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yi.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vr.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pf.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kp.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xm.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://yq.nszjky.cn

Py:   a and b or not c
来源：http://im.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://qm.nszjky.cn

JS:   a && b || !c
来源：http://cm.huanxung.cn

TS:   a && b || !c
来源：http://eo.colortex.cn

Java: a && b || !c
来源：http://nf.chemitech.net.cn

Go:   a && b || !c
来源：http://xh.asd995.cn

Ruby: a && b || !c
来源：http://fz.szxytkj.cn

C#:   a && b || !c
来源：http://xr.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ri.colortex.cn

Py:   if not data: return
来源：http://xp.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://kr.huanxung.cn

JS:   if (!data) return;
来源：http://kx.521024.cn

TS:   if (!data) return;
来源：http://px.huixiangedu.cn

Java: if (data == null) return;
来源：http://sn.shxzukj.cn

Go:   if data == nil { return }
来源：http://om.shxzukj.cn

Ruby: return if data.nil?
来源：http://vk.lnxyls.cn

C#:   if (data == null) return;
来源：http://gx.jctech888.com.cn

================================================================================
来源：http://ay.lnxyls.cn

C. 函数与作用域
来源：http://qq.yuntaijiaju.cn

================================================================================
来源：http://wz.nicolike.cn

[C01] 定义函数
来源：http://nx.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://fs.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://be.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://es.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bz.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ub.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://yz.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://st.hnjuh.cn

[C02] 默认参数
来源：http://nf.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://il.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lc.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ke.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cc.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tn.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hv.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://au.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://xk.haigaiapp.cn

[C03] 可变参数
来源：http://uu.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://iq.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gm.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ot.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oh.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://er.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ai.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ye.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kh.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ir.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jl.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ua.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nh.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hf.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://of.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://qf.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://fz.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://vf.haigaiapp.cn

[C05] 返回多个值
来源：http://bu.colortex.cn

Py:   return a, b
来源：http://qq.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://pr.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://en.nicolike.cn

TS:   return { a, b };
来源：http://lw.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yr.521024.cn

Go:   return a, b
来源：http://qo.newstarts.cn

Ruby: return a, b
来源：http://ot.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://oh.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://zi.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://rl.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lv.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://fv.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://di.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wt.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dy.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://lq.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wb.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://pm.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cb.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ma.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sj.hahajie.cn

TS:   arr.map(String)
来源：http://qa.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://px.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kv.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ei.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wg.bookmarksfly.cn

[C08] 闭包
来源：http://sb.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ov.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ku.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hd.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qa.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://av.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vc.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tm.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ju.yuntaijiaju.cn

[C09] 递归
来源：http://rs.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fi.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nx.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zq.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ns.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://en.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jm.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hk.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ov.huanxung.cn

[C10] 变量作用域
来源：http://ew.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pr.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uy.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bo.muxihuayi.cn

TS:   同 JS
来源：http://tn.huanxung.cn

Java: 方法内为块级作用域
来源：http://iz.gzmigu.cn

Go:   花括号块级作用域
来源：http://xa.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hh.nszjky.cn

C#:   块级作用域
来源：http://wi.nicolike.cn

[C11] 模块导入与导出
来源：http://us.hnjuh.cn

Py:   from module import func
来源：http://ta.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fw.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yy.hahajie.cn

Java: import java.util.List;
来源：http://fw.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mm.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://sk.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ai.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://ea.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://xy.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://vg.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://fp.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://sv.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fu.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ya.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ae.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vh.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://ed.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zf.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sj.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rp.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ip.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nd.shxzskj.cn

Go:   func add(a, b int) int
来源：http://ub.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ji.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tt.huixinmuqiang.cn

[C14] 泛型函数
来源：http://fo.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qg.lnxyls.cn

PHP:  // 无泛型
来源：http://qv.chemitech.net.cn

JS:   // 无泛型
来源：http://du.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yx.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nw.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://go.shxzukj.cn

Ruby: # 无泛型
来源：http://lv.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rl.newstarts.cn

[C15] 解构 / 展开参数
来源：http://hs.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qg.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://gq.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oj.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oe.nicolike.cn

Java: // 无解构
来源：http://be.9csxet.cn

Go:   // 无解构
来源：http://ad.shxzskj.cn

Ruby: a, b = pair
来源：http://qn.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ks.asd995.cn

[C16] 函数 / 方法重载
来源：http://zc.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cm.9csxet.cn

PHP:  // 无重载
来源：http://zv.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yi.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://bx.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wj.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://nk.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://dm.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rg.newstarts.cn

================================================================================
来源：http://cw.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://zf.nicolike.cn

================================================================================
来源：http://ds.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://yf.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fp.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://af.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sc.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://im.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ze.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://dc.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://wu.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mp.huanxung.cn

[D02] 追加元素到末尾
来源：http://fi.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ub.wgjwhj.cn

JS:   arr.push(4);
来源：http://sf.jctech888.com.cn

TS:   arr.push(4);
来源：http://bk.muxihuayi.cn

Java: list.add(4);
来源：http://ck.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://sl.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://zk.szxytkj.cn

C#:   list.Add(4);
来源：http://tl.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://un.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://wb.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ng.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://el.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://hf.asd995.cn

Java: list.add(0, 0);
来源：http://ns.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hb.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hd.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://qp.bjjhwx.cn

[D04] 删除元素
来源：http://py.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sy.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ot.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dl.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://fb.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kd.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zm.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oc.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ac.szsharing.cn

[D05] 访问与修改元素
来源：http://tj.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ut.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zf.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mz.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://lv.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://dy.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://ab.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mv.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ia.9csxet.cn

[D06] 数组长度
来源：http://qr.521024.cn

Py:   len(arr)
来源：http://yp.panjiajie.cn

PHP:  count($arr);
来源：http://zh.shxzukj.cn

JS:   arr.length
来源：http://dj.yuntaijiaju.cn

TS:   arr.length
来源：http://bg.jianghongdianzi.cn

Java: list.size();
来源：http://qk.haigaiapp.cn

Go:   len(arr)
来源：http://ug.huanxung.cn

Ruby: arr.length; arr.size
来源：http://sf.nicolike.cn

C#:   list.Count;
来源：http://wo.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://av.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ri.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://av.colortex.cn

JS:   arr.slice(1, 4);
来源：http://wz.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://af.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://by.huanxung.cn

Go:   arr[1:4]
来源：http://pn.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://ea.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://lb.hnjuh.cn

[D08] 合并两个数组
来源：http://al.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://tu.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://ox.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ak.jctech888.com.cn

TS:   [...a, ...b];
来源：http://hh.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ma.newstarts.cn

Go:   append(a, b...)
来源：http://uj.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://tn.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://qj.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://tt.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://dk.yuexingan06.cn

PHP:  sort($arr);
来源：http://jm.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wh.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sl.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vs.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pz.jctech888.com.cn

Ruby: arr.sort
来源：http://no.shtwfgs.cn

C#:   list.Sort();
来源：http://cz.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ah.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ve.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vg.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eq.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://og.9csxet.cn


<!-- 参考信息 -->