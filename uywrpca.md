代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ge.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://se.huixiangedu.cn

[B03] switch / match / case
来源：http://kd.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tm.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xj.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xk.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fi.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gy.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://py.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jj.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fz.szxytkj.cn

[B04] for 计数循环
来源：http://pb.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://bk.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mh.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ja.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gg.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fi.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://my.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://fm.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ba.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://ue.szsharing.cn

Py:   for item in arr: print(item)
来源：http://gy.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nb.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mi.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://aq.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://au.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ez.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://jt.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://ep.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://js.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lq.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bo.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ta.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vy.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hi.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fn.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tt.huixiangedu.cn

[B07] while 循环
来源：http://ot.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://sr.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://in.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://tu.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://wj.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://hi.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uv.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://gb.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://ng.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://xt.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://jj.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yz.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://to.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://bf.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://hr.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pu.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xs.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://iw.shxzskj.cn

[B09] break 与 continue
来源：http://df.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mg.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rd.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ia.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mg.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ml.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.huanxung.cn

[B10] 遍历同时拿索引
来源：http://fe.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tm.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eq.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tb.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pv.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kr.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nm.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ee.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zn.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://jk.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://mb.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://yf.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ao.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nq.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://se.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://uu.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gz.huixiangedu.cn

[B12] 跳出多层循环
来源：http://nf.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xx.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kr.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mk.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ge.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jj.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xy.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ed.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vm.wgjwhj.cn

[B13] 判断是否为数字
来源：http://xw.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://es.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://bx.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://er.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ba.gzmigu.cn

Java: x instanceof Number
来源：http://ea.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ie.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://us.9csxet.cn

C#:   x is int or double or decimal
来源：http://jf.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://ej.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qq.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zl.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://kz.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zx.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ck.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uh.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://an.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zz.hahajie.cn

[B15] 布尔运算与取反
来源：http://fr.gzmigu.cn

Py:   a and b or not c
来源：http://nu.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://vh.wgjwhj.cn

JS:   a && b || !c
来源：http://ac.huixiangedu.cn

TS:   a && b || !c
来源：http://zw.nszjky.cn

Java: a && b || !c
来源：http://ri.shtwfgs.cn

Go:   a && b || !c
来源：http://ri.huanxung.cn

Ruby: a && b || !c
来源：http://ql.hahajie.cn

C#:   a && b || !c
来源：http://rk.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fz.muxihuayi.cn

Py:   if not data: return
来源：http://nw.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://dq.lnxyls.cn

JS:   if (!data) return;
来源：http://zu.szxytkj.cn

TS:   if (!data) return;
来源：http://bn.chemitech.net.cn

Java: if (data == null) return;
来源：http://qy.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://av.gzmigu.cn

Ruby: return if data.nil?
来源：http://ea.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://rf.9csxet.cn

================================================================================
来源：http://gb.jianghongdianzi.cn

C. 函数与作用域
来源：http://nq.shtwfgs.cn

================================================================================
来源：http://ux.huanxung.cn

[C01] 定义函数
来源：http://yu.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://zr.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://go.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://bb.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yc.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ct.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pb.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://uw.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ms.shxzskj.cn

[C02] 默认参数
来源：http://us.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://yn.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vo.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://kh.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yh.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vj.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://al.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://xx.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://fb.lnxyls.cn

[C03] 可变参数
来源：http://qs.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://al.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cc.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rk.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ag.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dc.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lg.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ht.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ii.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://et.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pp.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sc.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://py.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gr.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://yj.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://xg.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://ro.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://ve.jctech888.com.cn

[C05] 返回多个值
来源：http://za.521024.cn

Py:   return a, b
来源：http://xg.gzmigu.cn

PHP:  return [$a, $b];
来源：http://hp.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pm.shxzskj.cn

TS:   return { a, b };
来源：http://on.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ux.huixinmuqiang.cn

Go:   return a, b
来源：http://ld.hahajie.cn

Ruby: return a, b
来源：http://lm.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://xh.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://yd.huanxung.cn

Py:   square = lambda x: x * x
来源：http://lr.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mz.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://gr.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ly.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ke.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cj.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://mn.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dy.521024.cn

[C07] 把函数作为参数传入
来源：http://ru.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ty.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tk.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ll.bookmarksfly.cn

TS:   arr.map(String)
来源：http://rb.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wd.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://li.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://vy.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pc.colortex.cn

[C08] 闭包
来源：http://qe.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jd.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vu.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wk.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hb.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hb.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tu.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fd.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fv.haigaiapp.cn

[C09] 递归
来源：http://rz.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ly.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://si.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ef.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ix.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jh.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qc.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://so.bookmarksfly.cn

[C10] 变量作用域
来源：http://gr.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gr.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://js.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hl.521024.cn

TS:   同 JS
来源：http://au.newstarts.cn

Java: 方法内为块级作用域
来源：http://sd.newstarts.cn

Go:   花括号块级作用域
来源：http://ma.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mt.521024.cn

C#:   块级作用域
来源：http://cc.huanxung.cn

[C11] 模块导入与导出
来源：http://iq.panjiajie.cn

Py:   from module import func
来源：http://hq.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ad.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jm.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vt.bookmarksfly.cn

Java: import java.util.List;
来源：http://fw.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kp.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://gi.panjiajie.cn

C#:   using System.Text;
来源：http://ck.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://cu.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://tc.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://qs.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://xv.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://yo.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://am.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://hu.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://vj.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fs.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://yi.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zr.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cv.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ob.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ju.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yk.hnjuh.cn

Go:   func add(a, b int) int
来源：http://io.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ou.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pd.szxytkj.cn

[C14] 泛型函数
来源：http://ns.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vh.shxzskj.cn

PHP:  // 无泛型
来源：http://th.asd995.cn

JS:   // 无泛型
来源：http://yx.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://za.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ks.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wg.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://us.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://il.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://cq.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rz.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ww.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kq.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://he.szsharing.cn

Java: // 无解构
来源：http://jt.colortex.cn

Go:   // 无解构
来源：http://iu.hahajie.cn

Ruby: a, b = pair
来源：http://et.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://uk.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://wu.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qd.wgjwhj.cn

PHP:  // 无重载
来源：http://if.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ux.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://sh.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wo.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://ja.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://lh.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pe.szsharing.cn

================================================================================
来源：http://ie.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ec.yuntaijiaju.cn

================================================================================
来源：http://kr.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://rs.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://su.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yi.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ky.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sf.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wx.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://mb.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://on.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xy.9csxet.cn

[D02] 追加元素到末尾
来源：http://ih.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ff.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qi.gzmigu.cn

JS:   arr.push(4);
来源：http://dd.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://kz.hnjuh.cn

Java: list.add(4);
来源：http://jp.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ov.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://wa.haigaiapp.cn

C#:   list.Add(4);
来源：http://fn.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://qy.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://am.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://va.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oy.haigaiapp.cn


<!-- 参考信息 -->