代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bx.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ta.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ru.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nq.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ex.wgjwhj.cn

[B04] for 计数循环
来源：http://fc.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://zu.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bc.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nk.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iv.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ip.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://fm.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ft.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://bu.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://jx.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hn.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jj.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gg.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ti.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sm.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://ve.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ra.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://zy.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ez.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://de.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zd.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zp.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ds.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qy.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pw.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ai.haigaiapp.cn

[B07] while 循环
来源：http://go.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://fz.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ec.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://fc.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ou.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://lp.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pj.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://oj.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://gm.colortex.cn

[B08] do-while（至少执行一次）
来源：http://qv.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://mh.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hp.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://fh.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://sj.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://rp.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cj.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rm.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://sn.huixinmuqiang.cn

[B09] break 与 continue
来源：http://po.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ci.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://no.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cq.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://md.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zk.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lq.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xv.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://fq.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jk.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gh.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://to.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hb.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tl.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://es.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kp.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sh.521024.cn

[B11] 生成数字序列 / 区间
来源：http://il.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ma.colortex.cn

PHP:  range(0, 10, 2);
来源：http://jg.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rm.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://je.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hp.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ks.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://fh.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://io.szxytkj.cn

[B12] 跳出多层循环
来源：http://kf.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kr.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xv.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qd.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nm.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ue.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xj.wgjwhj.cn

[B13] 判断是否为数字
来源：http://av.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://bj.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://bj.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dn.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qm.shxzukj.cn

Java: x instanceof Number
来源：http://fn.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fr.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://pb.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://cp.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://yj.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://no.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fk.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://sy.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://mc.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rg.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fn.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ez.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zd.gzmigu.cn

[B15] 布尔运算与取反
来源：http://cg.muxihuayi.cn

Py:   a and b or not c
来源：http://zz.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://oq.panjiajie.cn

JS:   a && b || !c
来源：http://qc.521024.cn

TS:   a && b || !c
来源：http://hd.jctech888.com.cn

Java: a && b || !c
来源：http://rh.521024.cn

Go:   a && b || !c
来源：http://ij.9csxet.cn

Ruby: a && b || !c
来源：http://tx.gzmigu.cn

C#:   a && b || !c
来源：http://gl.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hm.bookmarksfly.cn

Py:   if not data: return
来源：http://eq.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://jc.nicolike.cn

JS:   if (!data) return;
来源：http://zz.hahajie.cn

TS:   if (!data) return;
来源：http://tf.jctech888.com.cn

Java: if (data == null) return;
来源：http://qu.newstarts.cn

Go:   if data == nil { return }
来源：http://oy.asd995.cn

Ruby: return if data.nil?
来源：http://wz.newstarts.cn

C#:   if (data == null) return;
来源：http://go.yuexingan06.cn

================================================================================
来源：http://cw.shtwfgs.cn

C. 函数与作用域
来源：http://rt.jianghongdianzi.cn

================================================================================
来源：http://gh.hnjuh.cn

[C01] 定义函数
来源：http://bz.asd995.cn

Py:   def add(a, b): return a + b
来源：http://lj.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gr.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://di.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qq.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xj.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ra.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://xi.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vw.gzmigu.cn

[C02] 默认参数
来源：http://zg.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://bf.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fb.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://bx.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pc.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ai.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zs.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://qx.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ka.hnjuh.cn

[C03] 可变参数
来源：http://ws.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://ap.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fm.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kq.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hb.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zd.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ea.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oq.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mh.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ea.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ti.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ow.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zs.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ms.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://av.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://pw.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://zf.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://bh.yuexingan06.cn

[C05] 返回多个值
来源：http://xt.nicolike.cn

Py:   return a, b
来源：http://nz.hahajie.cn

PHP:  return [$a, $b];
来源：http://rd.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ph.shxzukj.cn

TS:   return { a, b };
来源：http://ae.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sf.huixiangedu.cn

Go:   return a, b
来源：http://vo.szsharing.cn

Ruby: return a, b
来源：http://dq.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://gn.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ve.nicolike.cn

Py:   square = lambda x: x * x
来源：http://lf.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://is.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://yo.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bj.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yz.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://pa.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://de.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://it.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pz.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xe.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gu.gzmigu.cn

TS:   arr.map(String)
来源：http://mg.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jc.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ey.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://dj.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kn.lnxyls.cn

[C08] 闭包
来源：http://jj.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ik.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tn.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dy.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yn.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xt.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mk.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lc.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qi.lnxyls.cn

[C09] 递归
来源：http://vv.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://db.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ln.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xw.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zd.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jt.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ag.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pr.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yy.shtwfgs.cn

[C10] 变量作用域
来源：http://aw.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gj.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cy.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kn.wgjwhj.cn

TS:   同 JS
来源：http://uu.hahajie.cn

Java: 方法内为块级作用域
来源：http://fk.huanxung.cn

Go:   花括号块级作用域
来源：http://os.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gg.jctech888.com.cn

C#:   块级作用域
来源：http://og.yuexingan06.cn

[C11] 模块导入与导出
来源：http://ub.yuntaijiaju.cn

Py:   from module import func
来源：http://yo.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sa.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://no.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uy.lnxyls.cn

Java: import java.util.List;
来源：http://mm.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kj.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://vn.bookmarksfly.cn

C#:   using System.Text;
来源：http://wv.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://wf.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://pm.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://ap.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://eg.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://ol.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ub.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://jd.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://xy.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ll.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://na.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ab.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jj.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nn.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ck.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gn.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ke.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ci.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vd.hahajie.cn

[C14] 泛型函数
来源：http://sp.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tw.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ic.jctech888.com.cn

JS:   // 无泛型
来源：http://ht.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ru.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lq.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ul.gzmigu.cn

Ruby: # 无泛型
来源：http://xb.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zh.nicolike.cn

[C15] 解构 / 展开参数
来源：http://cj.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ih.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://wf.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mz.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://og.jctech888.com.cn

Java: // 无解构
来源：http://fa.huanxung.cn

Go:   // 无解构
来源：http://bo.lnxyls.cn

Ruby: a, b = pair
来源：http://gp.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://dl.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://au.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zi.nszjky.cn

PHP:  // 无重载
来源：http://kf.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oh.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://nn.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ml.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://oy.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://qd.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://go.lnxyls.cn

================================================================================
来源：http://ok.colortex.cn

D. 数组 / 列表 / 集合
来源：http://vx.muxihuayi.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://wa.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://as.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oe.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://go.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ca.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jn.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://bi.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://fn.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iw.gzmigu.cn

[D02] 追加元素到末尾
来源：http://vb.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kb.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ew.shxzskj.cn

JS:   arr.push(4);
来源：http://kr.szsharing.cn

TS:   arr.push(4);
来源：http://ka.haigaiapp.cn

Java: list.add(4);
来源：http://nz.asd995.cn

Go:   arr = append(arr, 4)
来源：http://di.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://il.hahajie.cn

C#:   list.Add(4);
来源：http://tf.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ny.521024.cn

Py:   arr.insert(0, 0)
来源：http://hp.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://be.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xd.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://tj.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://xf.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yb.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xt.nszjky.cn


<!-- 参考信息 -->