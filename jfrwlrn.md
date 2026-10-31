代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nh.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wd.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pp.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pe.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://er.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oz.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ky.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://qt.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://qt.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nx.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gr.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vy.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://fh.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bn.colortex.cn

[B12] 跳出多层循环
来源：http://gb.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kj.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://su.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mc.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nf.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pi.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qr.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zq.jctech888.com.cn

[B13] 判断是否为数字
来源：http://oh.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://eb.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://qe.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rr.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eq.szxytkj.cn

Java: x instanceof Number
来源：http://jx.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qg.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://mb.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://oe.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://wa.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hf.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rk.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://pg.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://da.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fc.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rh.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yc.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://iw.szxytkj.cn

Py:   a and b or not c
来源：http://tf.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://qq.lnxyls.cn

JS:   a && b || !c
来源：http://kw.gzmigu.cn

TS:   a && b || !c
来源：http://at.szsharing.cn

Java: a && b || !c
来源：http://hn.hahajie.cn

Go:   a && b || !c
来源：http://dh.shxzukj.cn

Ruby: a && b || !c
来源：http://tk.wgjwhj.cn

C#:   a && b || !c
来源：http://wf.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ht.bookmarksfly.cn

Py:   if not data: return
来源：http://as.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://vb.chemitech.net.cn

JS:   if (!data) return;
来源：http://am.huixiangedu.cn

TS:   if (!data) return;
来源：http://jc.jctech888.com.cn

Java: if (data == null) return;
来源：http://ri.asd995.cn

Go:   if data == nil { return }
来源：http://ah.nszjky.cn

Ruby: return if data.nil?
来源：http://sf.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://aq.shxzskj.cn

================================================================================
来源：http://em.asd995.cn

C. 函数与作用域
来源：http://uq.asd995.cn

================================================================================
来源：http://ki.wgjwhj.cn

[C01] 定义函数
来源：http://pr.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://ov.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hp.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://st.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://za.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bf.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qt.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://dx.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xo.newstarts.cn

[C02] 默认参数
来源：http://ds.asd995.cn

Py:   def greet(name="World"): return name
来源：http://kx.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kt.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://uv.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fs.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nr.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cb.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://wm.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hj.gzmigu.cn

[C03] 可变参数
来源：http://fh.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://do.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jh.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tt.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yd.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pv.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ll.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mb.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ww.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fu.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ol.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lm.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://br.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://eg.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://sl.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://zj.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://ri.nszjky.cn

[C05] 返回多个值
来源：http://js.huanxung.cn

Py:   return a, b
来源：http://jo.shxzskj.cn

PHP:  return [$a, $b];
来源：http://kw.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ms.bjjhwx.cn

TS:   return { a, b };
来源：http://sc.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zo.chemitech.net.cn

Go:   return a, b
来源：http://xw.chemitech.net.cn

Ruby: return a, b
来源：http://cp.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://ya.asd995.cn

[C06] 匿名函数 / lambda
来源：http://va.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ul.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gp.hnjuh.cn

JS:   const square = x => x * x;
来源：http://dl.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ll.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ec.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bo.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://og.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://by.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ej.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kv.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ni.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lm.lnxyls.cn

TS:   arr.map(String)
来源：http://fd.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ms.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oo.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://yj.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vt.szxytkj.cn

[C08] 闭包
来源：http://uo.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ki.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vr.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://md.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://is.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cv.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://em.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ca.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://od.shxzukj.cn

[C09] 递归
来源：http://eo.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ow.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sm.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ma.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xu.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mk.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ab.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ng.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qt.shxzskj.cn

[C10] 变量作用域
来源：http://so.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hp.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dk.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gq.wgjwhj.cn

TS:   同 JS
来源：http://iu.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://no.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://pm.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://za.haigaiapp.cn

C#:   块级作用域
来源：http://uz.shtwfgs.cn

[C11] 模块导入与导出
来源：http://qe.muxihuayi.cn

Py:   from module import func
来源：http://ls.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jk.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sy.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jz.nicolike.cn

Java: import java.util.List;
来源：http://wd.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://za.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://li.szsharing.cn

C#:   using System.Text;
来源：http://pm.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://dm.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://wa.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://kz.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://dj.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://wz.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qt.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://dp.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://dv.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dk.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://cq.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://as.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rt.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wr.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ed.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://el.nszjky.cn

Go:   func add(a, b int) int
来源：http://vz.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ce.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ex.shxzukj.cn

[C14] 泛型函数
来源：http://cp.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ca.chemitech.net.cn

PHP:  // 无泛型
来源：http://gl.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ti.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ri.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rh.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gx.huanxung.cn

Ruby: # 无泛型
来源：http://gv.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ci.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://fl.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yf.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://sg.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eg.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wc.gzmigu.cn

Java: // 无解构
来源：http://ok.szsharing.cn

Go:   // 无解构
来源：http://tj.wgjwhj.cn

Ruby: a, b = pair
来源：http://ox.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://eg.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://lb.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ph.hahajie.cn

PHP:  // 无重载
来源：http://ob.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://re.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://ap.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://be.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://vx.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://vk.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kt.jctech888.com.cn

================================================================================
来源：http://rd.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://ua.shxzskj.cn

================================================================================
来源：http://ig.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://uc.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ha.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zv.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qf.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ht.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fb.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://wn.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://lz.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kp.colortex.cn

[D02] 追加元素到末尾
来源：http://ts.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kd.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rm.wgjwhj.cn

JS:   arr.push(4);
来源：http://in.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ba.asd995.cn

Java: list.add(4);
来源：http://hm.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://jr.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://dx.jctech888.com.cn

C#:   list.Add(4);
来源：http://zw.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://tz.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://fr.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ug.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ve.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://qa.9csxet.cn

Java: list.add(0, 0);
来源：http://es.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mq.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uk.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://cn.hahajie.cn

[D04] 删除元素
来源：http://jy.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jc.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cj.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ku.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://qc.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dh.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xg.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wo.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bo.bjjhwx.cn

[D05] 访问与修改元素
来源：http://mm.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cc.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bw.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ec.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://vp.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://cp.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://qv.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xu.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.szsharing.cn

[D06] 数组长度
来源：http://cv.shxzukj.cn

Py:   len(arr)
来源：http://ic.bjjhwx.cn

PHP:  count($arr);
来源：http://yq.colortex.cn

JS:   arr.length
来源：http://pm.colortex.cn

TS:   arr.length
来源：http://jt.bjjhwx.cn

Java: list.size();
来源：http://nt.szsharing.cn

Go:   len(arr)
来源：http://wu.szsharing.cn

Ruby: arr.length; arr.size
来源：http://gy.yuntaijiaju.cn

C#:   list.Count;
来源：http://ub.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://wv.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yo.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zm.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://nk.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://iy.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://he.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://cw.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://vw.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://ti.gzmigu.cn

[D08] 合并两个数组
来源：http://iy.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://se.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://mp.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ve.gzmigu.cn

TS:   [...a, ...b];
来源：http://ft.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cy.lnxyls.cn

Go:   append(a, b...)
来源：http://il.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://cf.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://gt.gzmigu.cn

[D09] 排序（升序）
来源：http://ne.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://at.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://lv.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ls.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sy.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kg.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jw.panjiajie.cn

Ruby: arr.sort
来源：http://bq.szxytkj.cn

C#:   list.Sort();
来源：http://ab.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jq.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pa.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gq.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://le.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tf.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://br.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zb.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yy.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lq.huanxung.cn


<!-- 参考信息 -->