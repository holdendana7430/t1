代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jy.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ab.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xa.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uc.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://fr.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xg.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yc.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xy.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aa.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fx.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jd.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kp.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rf.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://xu.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://ap.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://nz.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vt.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nz.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oh.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hq.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://su.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aa.jctech888.com.cn

[B12] 跳出多层循环
来源：http://yt.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ic.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vr.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fe.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sj.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ev.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sk.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pf.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sl.shxzukj.cn

[B13] 判断是否为数字
来源：http://ht.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://xd.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://xc.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kr.nicolike.cn

Java: x instanceof Number
来源：http://qf.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zh.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://xu.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://pm.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://ky.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tr.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://an.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://au.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://mq.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vp.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://av.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sg.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lw.huanxung.cn

[B15] 布尔运算与取反
来源：http://mj.521024.cn

Py:   a and b or not c
来源：http://js.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://om.gzmigu.cn

JS:   a && b || !c
来源：http://ne.chemitech.net.cn

TS:   a && b || !c
来源：http://ve.521024.cn

Java: a && b || !c
来源：http://dw.hahajie.cn

Go:   a && b || !c
来源：http://sb.9csxet.cn

Ruby: a && b || !c
来源：http://wn.hahajie.cn

C#:   a && b || !c
来源：http://sr.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://er.shtwfgs.cn

Py:   if not data: return
来源：http://mn.521024.cn

PHP:  if (!$data) { return; }
来源：http://bm.szsharing.cn

JS:   if (!data) return;
来源：http://ms.chemitech.net.cn

TS:   if (!data) return;
来源：http://wd.panjiajie.cn

Java: if (data == null) return;
来源：http://xu.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://eb.colortex.cn

Ruby: return if data.nil?
来源：http://ki.shtwfgs.cn

C#:   if (data == null) return;
来源：http://hw.colortex.cn

================================================================================
来源：http://bd.szsharing.cn

C. 函数与作用域
来源：http://fv.wgjwhj.cn

================================================================================
来源：http://rj.nszjky.cn

[C01] 定义函数
来源：http://xx.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://zs.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fh.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://me.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uz.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iy.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ni.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://bc.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ww.chemitech.net.cn

[C02] 默认参数
来源：http://zq.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://cv.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ic.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://fa.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kr.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vz.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pf.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://ff.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://sq.nszjky.cn

[C03] 可变参数
来源：http://zi.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://if.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lb.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hu.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xz.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xf.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xb.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ln.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bm.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://yd.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dk.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ix.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hc.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ox.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://zd.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://kv.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ql.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://hp.shtwfgs.cn

[C05] 返回多个值
来源：http://kv.huanxung.cn

Py:   return a, b
来源：http://de.colortex.cn

PHP:  return [$a, $b];
来源：http://ka.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ez.huixiangedu.cn

TS:   return { a, b };
来源：http://rp.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wm.chemitech.net.cn

Go:   return a, b
来源：http://dc.shxzskj.cn

Ruby: return a, b
来源：http://in.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://bi.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://hx.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://rf.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xv.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://at.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://tg.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rv.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://al.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://xh.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rh.nszjky.cn

[C07] 把函数作为参数传入
来源：http://nm.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ek.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kq.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oj.lnxyls.cn

TS:   arr.map(String)
来源：http://hi.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ou.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wl.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://mr.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rd.haigaiapp.cn

[C08] 闭包
来源：http://sp.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jn.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uk.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ja.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ql.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yz.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gn.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://la.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://br.huixiangedu.cn

[C09] 递归
来源：http://nk.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ia.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iq.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qe.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ha.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sb.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cf.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cv.bookmarksfly.cn

[C10] 变量作用域
来源：http://sc.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jj.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gn.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hp.lnxyls.cn

TS:   同 JS
来源：http://vp.szsharing.cn

Java: 方法内为块级作用域
来源：http://nn.shtwfgs.cn

Go:   花括号块级作用域
来源：http://iu.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rw.yuntaijiaju.cn

C#:   块级作用域
来源：http://gb.nszjky.cn

[C11] 模块导入与导出
来源：http://eq.huixinmuqiang.cn

Py:   from module import func
来源：http://vb.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sv.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kx.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oy.nszjky.cn

Java: import java.util.List;
来源：http://qb.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hs.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://yo.wgjwhj.cn

C#:   using System.Text;
来源：http://ay.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ut.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://vd.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://rl.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://ky.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://uv.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lx.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ry.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ja.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hk.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://jm.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://py.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jt.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ti.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zf.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://fb.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://to.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pa.nicolike.cn

[C14] 泛型函数
来源：http://la.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iz.newstarts.cn

PHP:  // 无泛型
来源：http://za.nszjky.cn

JS:   // 无泛型
来源：http://xs.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sv.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kd.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dy.bookmarksfly.cn

Ruby: # 无泛型
来源：http://al.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ot.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ya.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wo.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://hs.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fy.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pw.gzmigu.cn

Java: // 无解构
来源：http://nn.szsharing.cn

Go:   // 无解构
来源：http://lm.newstarts.cn

Ruby: a, b = pair
来源：http://hf.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://rg.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://si.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ju.bjjhwx.cn

PHP:  // 无重载
来源：http://py.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ay.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ym.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ij.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://aw.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xl.asd995.cn

================================================================================
来源：http://ve.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://po.9csxet.cn

================================================================================
来源：http://tc.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://ru.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fa.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ld.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uj.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qd.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ly.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://ez.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://pi.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uj.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://fi.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xq.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ch.szsharing.cn

JS:   arr.push(4);
来源：http://dy.9csxet.cn

TS:   arr.push(4);
来源：http://zb.muxihuayi.cn

Java: list.add(4);
来源：http://ic.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://bz.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://xs.9csxet.cn

C#:   list.Add(4);
来源：http://jo.newstarts.cn

[D03] 在指定位置插入元素
来源：http://xm.521024.cn

Py:   arr.insert(0, 0)
来源：http://ou.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ic.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mf.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://am.hahajie.cn

Java: list.add(0, 0);
来源：http://ot.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zr.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://py.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ih.yuntaijiaju.cn

[D04] 删除元素
来源：http://jm.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vp.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rd.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jf.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://yg.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rg.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wd.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rb.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ox.gzmigu.cn

[D05] 访问与修改元素
来源：http://ds.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rx.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://my.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sc.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://ht.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://pa.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://xq.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cz.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://al.newstarts.cn

[D06] 数组长度
来源：http://vk.nicolike.cn

Py:   len(arr)
来源：http://tv.9csxet.cn

PHP:  count($arr);
来源：http://nv.521024.cn

JS:   arr.length
来源：http://cq.asd995.cn

TS:   arr.length
来源：http://mu.shtwfgs.cn

Java: list.size();
来源：http://pe.haigaiapp.cn

Go:   len(arr)
来源：http://ip.newstarts.cn

Ruby: arr.length; arr.size
来源：http://gz.9csxet.cn

C#:   list.Count;
来源：http://gq.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://xt.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ln.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qy.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://xf.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://iu.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://bu.9csxet.cn

Go:   arr[1:4]
来源：http://mv.asd995.cn

Ruby: arr[1, 3]
来源：http://xe.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://ex.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://zn.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://eq.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://pr.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fb.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://gp.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sy.521024.cn

Go:   append(a, b...)
来源：http://nx.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://xi.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://xp.szsharing.cn

[D09] 排序（升序）
来源：http://tc.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://wo.huanxung.cn

PHP:  sort($arr);
来源：http://lp.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qn.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://np.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ft.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ca.hahajie.cn

Ruby: arr.sort
来源：http://dl.szsharing.cn

C#:   list.Sort();
来源：http://ys.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qg.bookmarksfly.cn


<!-- 参考信息 -->