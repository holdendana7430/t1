代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fr.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qs.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lw.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vy.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ty.szsharing.cn

[B04] for 计数循环
来源：http://ix.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://pc.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sz.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://we.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kv.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wy.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ne.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://zj.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://tc.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://os.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xv.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yj.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vr.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pm.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://op.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://zv.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xw.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://kl.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sb.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://es.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mw.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hu.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://od.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jz.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bd.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cj.hahajie.cn

[B07] while 循环
来源：http://xm.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://zt.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zc.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://bw.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://qj.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://yk.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vy.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://om.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://dt.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://fi.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://ic.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://je.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://qc.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://wi.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://fq.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dm.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tq.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://xk.muxihuayi.cn

[B09] break 与 continue
来源：http://gn.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xb.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vw.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vz.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oj.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ya.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://xe.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jp.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rl.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vt.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sc.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xr.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ph.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yk.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://de.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://tx.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://ht.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://hf.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ye.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://km.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fs.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://lm.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vv.szxytkj.cn

[B12] 跳出多层循环
来源：http://vv.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fe.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wg.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vf.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pb.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oj.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://re.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kb.haigaiapp.cn

[B13] 判断是否为数字
来源：http://vh.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://dl.huanxung.cn

PHP:  is_numeric($x)
来源：http://rs.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://my.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.jianghongdianzi.cn

Java: x instanceof Number
来源：http://tj.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iy.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://sx.colortex.cn

C#:   x is int or double or decimal
来源：http://gl.colortex.cn

[B14] 判断值是否在集合内
来源：http://lx.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yh.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ai.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://ye.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://kn.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rb.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hp.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mx.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ga.asd995.cn

[B15] 布尔运算与取反
来源：http://lb.hahajie.cn

Py:   a and b or not c
来源：http://pj.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://gm.bookmarksfly.cn

JS:   a && b || !c
来源：http://ah.shxzukj.cn

TS:   a && b || !c
来源：http://pk.muxihuayi.cn

Java: a && b || !c
来源：http://nb.yuexingan06.cn

Go:   a && b || !c
来源：http://ef.nszjky.cn

Ruby: a && b || !c
来源：http://oh.haigaiapp.cn

C#:   a && b || !c
来源：http://zg.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yp.chemitech.net.cn

Py:   if not data: return
来源：http://mo.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://pj.panjiajie.cn

JS:   if (!data) return;
来源：http://sk.lnxyls.cn

TS:   if (!data) return;
来源：http://uc.muxihuayi.cn

Java: if (data == null) return;
来源：http://hs.szxytkj.cn

Go:   if data == nil { return }
来源：http://sz.yuexingan06.cn

Ruby: return if data.nil?
来源：http://qj.nicolike.cn

C#:   if (data == null) return;
来源：http://wv.nszjky.cn

================================================================================
来源：http://kf.bookmarksfly.cn

C. 函数与作用域
来源：http://rq.jianghongdianzi.cn

================================================================================
来源：http://uh.nszjky.cn

[C01] 定义函数
来源：http://fd.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ds.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://np.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://bw.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fh.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ts.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ux.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://vt.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nz.yuntaijiaju.cn

[C02] 默认参数
来源：http://bj.colortex.cn

Py:   def greet(name="World"): return name
来源：http://sw.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ok.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://xs.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fn.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ql.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://be.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://lz.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://xd.9csxet.cn

[C03] 可变参数
来源：http://pi.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://qq.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zr.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://md.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dr.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vb.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hy.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ey.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ec.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://zd.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hd.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jq.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://td.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cw.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ky.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://yg.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://yl.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://ux.shxzukj.cn

[C05] 返回多个值
来源：http://ww.gzmigu.cn

Py:   return a, b
来源：http://ps.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://jt.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zg.chemitech.net.cn

TS:   return { a, b };
来源：http://ec.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cu.haigaiapp.cn

Go:   return a, b
来源：http://ib.shxzskj.cn

Ruby: return a, b
来源：http://im.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://nn.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://xu.asd995.cn

Py:   square = lambda x: x * x
来源：http://zc.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ij.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://sz.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://vx.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jn.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kz.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://kb.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ub.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ba.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gx.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ek.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ua.szsharing.cn

TS:   arr.map(String)
来源：http://fg.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vy.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zf.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://og.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://df.nszjky.cn

[C08] 闭包
来源：http://rq.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xb.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jo.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ht.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iz.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zh.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gn.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wk.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wx.szsharing.cn

[C09] 递归
来源：http://hk.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ch.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bo.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yd.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ky.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://en.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://it.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://id.huixinmuqiang.cn

[C10] 变量作用域
来源：http://tj.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ih.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yh.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oi.huixiangedu.cn

TS:   同 JS
来源：http://lo.hnjuh.cn

Java: 方法内为块级作用域
来源：http://vb.9csxet.cn

Go:   花括号块级作用域
来源：http://hm.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qt.hnjuh.cn

C#:   块级作用域
来源：http://ds.yuexingan06.cn

[C11] 模块导入与导出
来源：http://lh.jianghongdianzi.cn

Py:   from module import func
来源：http://xo.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tu.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sn.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://so.szsharing.cn

Java: import java.util.List;
来源：http://ze.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ky.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://am.haigaiapp.cn

C#:   using System.Text;
来源：http://pu.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://ne.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://uo.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://nv.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://mo.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://rw.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yt.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://gr.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://lj.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ul.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://zk.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iw.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lc.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wq.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yw.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rk.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ba.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ek.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fd.gzmigu.cn

[C14] 泛型函数
来源：http://gz.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sw.shxzukj.cn

PHP:  // 无泛型
来源：http://in.hnjuh.cn

JS:   // 无泛型
来源：http://we.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vi.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mb.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kj.colortex.cn

Ruby: # 无泛型
来源：http://fc.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cl.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://wk.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vs.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://lz.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cy.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qr.haigaiapp.cn

Java: // 无解构
来源：http://vq.szxytkj.cn

Go:   // 无解构
来源：http://dk.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://ep.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://mr.huanxung.cn

[C16] 函数 / 方法重载
来源：http://gd.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qh.huanxung.cn

PHP:  // 无重载
来源：http://oz.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xn.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://em.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jc.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://na.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://hm.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ie.jianghongdianzi.cn

================================================================================
来源：http://yn.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://uj.haigaiapp.cn

================================================================================
来源：http://fy.asd995.cn

[D01] 创建数组 / 列表
来源：http://zz.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pc.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uj.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ds.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lk.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gm.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ug.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://ra.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jk.521024.cn

[D02] 追加元素到末尾
来源：http://sz.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ty.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yb.nszjky.cn

JS:   arr.push(4);
来源：http://ea.shxzskj.cn

TS:   arr.push(4);
来源：http://ys.shxzukj.cn

Java: list.add(4);
来源：http://aj.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://mt.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://tv.shxzukj.cn

C#:   list.Add(4);
来源：http://gi.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://vi.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://md.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://go.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://db.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://mx.colortex.cn

Java: list.add(0, 0);
来源：http://ls.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fn.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yv.huixiangedu.cn


<!-- 参考信息 -->