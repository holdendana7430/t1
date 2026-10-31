代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mu.nicolike.cn

[B02] 多分支 else if / elif
来源：http://yl.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://td.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fi.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://po.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tr.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ou.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ez.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hc.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.shtwfgs.cn

[B03] switch / match / case
来源：http://lk.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hu.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yl.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lc.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ch.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ac.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ov.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hf.huixiangedu.cn

[B04] for 计数循环
来源：http://oi.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://wj.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ym.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ej.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qd.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fv.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uh.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://qm.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fd.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://tm.newstarts.cn

Py:   for item in arr: print(item)
来源：http://om.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hs.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lf.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uy.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kf.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ax.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://wk.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ag.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://kn.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tt.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ef.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vr.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ci.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qz.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zl.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bs.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://if.shxzukj.cn

[B07] while 循环
来源：http://jp.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://qb.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hf.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://zs.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://tc.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://cc.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nn.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://ag.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://of.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://gu.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://xo.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://if.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://qf.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://kj.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ye.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://md.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fg.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://kl.haigaiapp.cn

[B09] break 与 continue
来源：http://ez.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hb.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ve.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ih.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://on.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ge.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nf.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wk.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pm.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uv.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qc.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xz.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zq.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ov.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://vg.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://hg.521024.cn

PHP:  range(0, 10, 2);
来源：http://fr.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bg.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://so.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xa.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gp.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://il.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cl.muxihuayi.cn

[B12] 跳出多层循环
来源：http://jp.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ap.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sc.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cq.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://if.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://of.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mw.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vr.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://oj.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://sf.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://yx.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wr.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dl.huixinmuqiang.cn

Java: x instanceof Number
来源：http://df.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jp.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://tw.huanxung.cn

C#:   x is int or double or decimal
来源：http://vm.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ny.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ka.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mq.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://zw.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://vy.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ba.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zz.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tr.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xc.lnxyls.cn

[B15] 布尔运算与取反
来源：http://im.nicolike.cn

Py:   a and b or not c
来源：http://xh.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://vj.shxzskj.cn

JS:   a && b || !c
来源：http://wo.hahajie.cn

TS:   a && b || !c
来源：http://hf.jctech888.com.cn

Java: a && b || !c
来源：http://bi.bjjhwx.cn

Go:   a && b || !c
来源：http://hn.haigaiapp.cn

Ruby: a && b || !c
来源：http://gv.nicolike.cn

C#:   a && b || !c
来源：http://nn.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bm.muxihuayi.cn

Py:   if not data: return
来源：http://mu.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://ab.hahajie.cn

JS:   if (!data) return;
来源：http://sv.shtwfgs.cn

TS:   if (!data) return;
来源：http://av.szsharing.cn

Java: if (data == null) return;
来源：http://un.bjjhwx.cn

Go:   if data == nil { return }
来源：http://ef.szxytkj.cn

Ruby: return if data.nil?
来源：http://ai.chemitech.net.cn

C#:   if (data == null) return;
来源：http://lc.gzmigu.cn

================================================================================
来源：http://ty.hahajie.cn

C. 函数与作用域
来源：http://dy.9csxet.cn

================================================================================
来源：http://to.bjjhwx.cn

[C01] 定义函数
来源：http://fn.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://au.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ny.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://vg.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ei.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://np.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xl.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ak.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vl.shxzukj.cn

[C02] 默认参数
来源：http://fb.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://ki.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bg.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://yb.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bl.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kz.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wd.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://sh.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://dq.shtwfgs.cn

[C03] 可变参数
来源：http://gx.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://tj.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://is.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://og.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://il.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://av.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ae.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qa.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eq.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://qm.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xa.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fe.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hm.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uq.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://na.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://gx.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://dn.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://at.yuexingan06.cn

[C05] 返回多个值
来源：http://jn.colortex.cn

Py:   return a, b
来源：http://jb.9csxet.cn

PHP:  return [$a, $b];
来源：http://nt.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vf.nszjky.cn

TS:   return { a, b };
来源：http://me.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nt.szsharing.cn

Go:   return a, b
来源：http://gp.shxzskj.cn

Ruby: return a, b
来源：http://rz.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://in.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://nt.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://ek.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ki.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://bj.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://qc.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vc.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hc.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://uz.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bc.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://vh.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ye.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wn.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eo.muxihuayi.cn

TS:   arr.map(String)
来源：http://be.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://so.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vm.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://cw.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ba.colortex.cn

[C08] 闭包
来源：http://fi.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bk.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ua.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sg.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nd.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oe.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ya.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ml.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ux.jctech888.com.cn

[C09] 递归
来源：http://lk.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gn.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tt.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pv.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cd.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vl.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://to.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tf.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ji.asd995.cn

[C10] 变量作用域
来源：http://xq.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lp.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nc.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mx.newstarts.cn

TS:   同 JS
来源：http://ik.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://cz.hahajie.cn

Go:   花括号块级作用域
来源：http://cg.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://la.szsharing.cn

C#:   块级作用域
来源：http://ap.shxzskj.cn

[C11] 模块导入与导出
来源：http://sk.jianghongdianzi.cn

Py:   from module import func
来源：http://xi.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jg.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mx.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dl.yuntaijiaju.cn

Java: import java.util.List;
来源：http://bh.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://re.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ab.muxihuayi.cn

C#:   using System.Text;
来源：http://yg.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://kq.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://sw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://vr.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://dx.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://ds.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ab.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://bf.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://gi.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://re.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ns.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hp.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wy.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://js.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pz.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://am.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://tu.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://du.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wp.bjjhwx.cn

[C14] 泛型函数
来源：http://be.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zv.bjjhwx.cn

PHP:  // 无泛型
来源：http://nl.shxzskj.cn

JS:   // 无泛型
来源：http://av.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rz.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xq.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fa.gzmigu.cn

Ruby: # 无泛型
来源：http://rx.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tq.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://hg.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kg.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://tk.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xo.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ja.bookmarksfly.cn

Java: // 无解构
来源：http://fl.newstarts.cn

Go:   // 无解构
来源：http://jl.521024.cn

Ruby: a, b = pair
来源：http://jc.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://tb.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://vw.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tl.nszjky.cn

PHP:  // 无重载
来源：http://ad.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wc.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://zx.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qe.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://fq.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://tp.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pp.yuntaijiaju.cn

================================================================================
来源：http://xo.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://am.wgjwhj.cn

================================================================================
来源：http://xc.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://te.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dw.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iq.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mk.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://or.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tb.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://xp.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://zh.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vd.lnxyls.cn

[D02] 追加元素到末尾
来源：http://sa.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sg.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xy.wgjwhj.cn

JS:   arr.push(4);
来源：http://hx.9csxet.cn

TS:   arr.push(4);
来源：http://ym.muxihuayi.cn


<!-- 参考信息 -->