代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://di.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xw.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lk.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kl.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://kq.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sr.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ei.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cb.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cq.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wq.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rx.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://co.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://th.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://mn.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://vt.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://hr.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qv.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sy.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ui.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vc.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://pr.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zc.colortex.cn

[B12] 跳出多层循环
来源：http://rj.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ol.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ky.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://da.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://la.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ca.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uf.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://il.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ez.panjiajie.cn

[B13] 判断是否为数字
来源：http://pu.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://rx.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://pb.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kl.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.colortex.cn

Java: x instanceof Number
来源：http://et.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jz.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://cj.shxzskj.cn

C#:   x is int or double or decimal
来源：http://gj.nicolike.cn

[B14] 判断值是否在集合内
来源：http://qv.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ky.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ac.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://oy.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://ri.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rn.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ur.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mt.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cu.nszjky.cn

[B15] 布尔运算与取反
来源：http://xp.szsharing.cn

Py:   a and b or not c
来源：http://tb.nszjky.cn

PHP:  $a && $b || !$c
来源：http://lb.yuntaijiaju.cn

JS:   a && b || !c
来源：http://cd.nszjky.cn

TS:   a && b || !c
来源：http://zj.wgjwhj.cn

Java: a && b || !c
来源：http://zb.panjiajie.cn

Go:   a && b || !c
来源：http://pu.szxytkj.cn

Ruby: a && b || !c
来源：http://pw.bjjhwx.cn

C#:   a && b || !c
来源：http://ct.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ro.huanxung.cn

Py:   if not data: return
来源：http://rp.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://zj.gzmigu.cn

JS:   if (!data) return;
来源：http://my.hnjuh.cn

TS:   if (!data) return;
来源：http://uk.gzmigu.cn

Java: if (data == null) return;
来源：http://vq.521024.cn

Go:   if data == nil { return }
来源：http://yc.shxzukj.cn

Ruby: return if data.nil?
来源：http://td.szxytkj.cn

C#:   if (data == null) return;
来源：http://wj.wgjwhj.cn

================================================================================
来源：http://uo.panjiajie.cn

C. 函数与作用域
来源：http://qx.huixinmuqiang.cn

================================================================================
来源：http://kc.yuexingan06.cn

[C01] 定义函数
来源：http://ek.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://bh.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ns.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://aq.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pw.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hk.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ao.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ly.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://by.szxytkj.cn

[C02] 默认参数
来源：http://tn.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://hf.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ik.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://au.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ft.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pn.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://up.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://lq.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://dk.muxihuayi.cn

[C03] 可变参数
来源：http://gy.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://ep.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rn.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zf.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jw.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bh.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ix.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rl.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://th.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rc.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bd.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sv.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://af.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hb.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://aa.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://eb.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://sc.jianghongdianzi.cn

[C05] 返回多个值
来源：http://iv.nszjky.cn

Py:   return a, b
来源：http://pa.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://nh.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hd.haigaiapp.cn

TS:   return { a, b };
来源：http://wt.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://as.bookmarksfly.cn

Go:   return a, b
来源：http://de.shtwfgs.cn

Ruby: return a, b
来源：http://ca.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ue.asd995.cn

[C06] 匿名函数 / lambda
来源：http://pz.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://qa.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://by.lnxyls.cn

JS:   const square = x => x * x;
来源：http://tg.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://un.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ar.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cv.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ut.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ox.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://ki.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kc.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://os.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mk.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://ww.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://as.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cy.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ei.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ts.521024.cn

[C08] 闭包
来源：http://fj.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rv.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gv.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ha.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oi.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uv.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hp.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dn.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ep.colortex.cn

[C09] 递归
来源：http://so.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://os.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zx.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jl.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://me.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ul.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ao.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fb.bjjhwx.cn

[C10] 变量作用域
来源：http://sr.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://on.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ym.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ou.szxytkj.cn

TS:   同 JS
来源：http://fe.nicolike.cn

Java: 方法内为块级作用域
来源：http://ox.chemitech.net.cn

Go:   花括号块级作用域
来源：http://cd.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://om.huixiangedu.cn

C#:   块级作用域
来源：http://gy.9csxet.cn

[C11] 模块导入与导出
来源：http://nt.asd995.cn

Py:   from module import func
来源：http://ey.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zu.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uh.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rb.wgjwhj.cn

Java: import java.util.List;
来源：http://uu.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qt.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ke.lnxyls.cn

C#:   using System.Text;
来源：http://ju.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://qi.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://za.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://ln.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://fk.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://sp.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tf.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://tg.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://wp.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tv.521024.cn

[C13] 类型声明 / 类型注解
来源：http://wd.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ec.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tm.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://to.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ej.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://uw.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fc.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sj.newstarts.cn

[C14] 泛型函数
来源：http://pw.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://py.chemitech.net.cn

PHP:  // 无泛型
来源：http://xx.yuntaijiaju.cn

JS:   // 无泛型
来源：http://om.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lb.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hi.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vz.chemitech.net.cn

Ruby: # 无泛型
来源：http://xb.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zt.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://ar.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ch.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://ne.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kn.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xn.jianghongdianzi.cn

Java: // 无解构
来源：http://px.lnxyls.cn

Go:   // 无解构
来源：http://md.haigaiapp.cn

Ruby: a, b = pair
来源：http://ss.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://mu.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://st.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sk.bjjhwx.cn

PHP:  // 无重载
来源：http://zn.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zh.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://kt.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jf.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://ru.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://mw.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aq.shtwfgs.cn

================================================================================
来源：http://we.colortex.cn

D. 数组 / 列表 / 集合
来源：http://wf.newstarts.cn

================================================================================
来源：http://zt.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://jj.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mb.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fs.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ht.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sw.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nj.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://tw.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://mu.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://br.nicolike.cn

[D02] 追加元素到末尾
来源：http://gr.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tj.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vu.huanxung.cn

JS:   arr.push(4);
来源：http://ew.hahajie.cn

TS:   arr.push(4);
来源：http://zl.nicolike.cn

Java: list.add(4);
来源：http://ps.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://fz.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://se.9csxet.cn

C#:   list.Add(4);
来源：http://fp.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://py.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://zm.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mk.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aw.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://vq.huanxung.cn

Java: list.add(0, 0);
来源：http://bb.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://op.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gi.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://ta.nicolike.cn

[D04] 删除元素
来源：http://rk.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yp.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zi.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zx.521024.cn

TS:   arr.splice(0, 1);
来源：http://ee.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ks.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mp.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ao.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hl.nicolike.cn

[D05] 访问与修改元素
来源：http://dg.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cx.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ci.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dh.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://ud.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://kq.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://oj.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://va.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uy.jianghongdianzi.cn

[D06] 数组长度
来源：http://xu.szsharing.cn

Py:   len(arr)
来源：http://iy.gzmigu.cn

PHP:  count($arr);
来源：http://qe.bjjhwx.cn

JS:   arr.length
来源：http://rq.asd995.cn

TS:   arr.length
来源：http://id.colortex.cn

Java: list.size();
来源：http://wd.yuntaijiaju.cn

Go:   len(arr)
来源：http://pj.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://ci.nszjky.cn

C#:   list.Count;
来源：http://fe.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://tn.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fp.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mk.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://sa.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://tj.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ld.colortex.cn

Go:   arr[1:4]
来源：http://ba.gzmigu.cn

Ruby: arr[1, 3]
来源：http://rj.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://jw.nicolike.cn

[D08] 合并两个数组
来源：http://nz.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://dc.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://xc.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://za.colortex.cn

TS:   [...a, ...b];
来源：http://pv.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ot.hahajie.cn

Go:   append(a, b...)
来源：http://mj.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://hr.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://dk.huanxung.cn

[D09] 排序（升序）
来源：http://vg.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ya.huanxung.cn

PHP:  sort($arr);
来源：http://qt.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sq.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ti.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tk.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xp.szxytkj.cn

Ruby: arr.sort
来源：http://bj.shtwfgs.cn

C#:   list.Sort();
来源：http://df.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tf.nszjky.cn


<!-- 参考信息 -->