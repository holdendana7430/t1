代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ad.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cb.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zt.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.huanxung.cn

[B10] 遍历同时拿索引
来源：http://kz.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fm.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pa.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://to.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ri.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://db.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dw.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qz.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mv.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://vy.521024.cn

Py:   list(range(0, 10, 2))
来源：http://nc.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://li.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ox.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ir.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nk.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ox.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://ub.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://al.hnjuh.cn

[B12] 跳出多层循环
来源：http://wk.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fq.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wg.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mz.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kf.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mn.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hq.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rf.shtwfgs.cn

[B13] 判断是否为数字
来源：http://sb.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://rt.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://se.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ja.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gm.szsharing.cn

Java: x instanceof Number
来源：http://jc.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gx.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://yg.hnjuh.cn

C#:   x is int or double or decimal
来源：http://el.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ky.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wg.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jn.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://vm.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://vb.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qf.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yw.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nf.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bc.szxytkj.cn

[B15] 布尔运算与取反
来源：http://tm.gzmigu.cn

Py:   a and b or not c
来源：http://cj.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://zv.panjiajie.cn

JS:   a && b || !c
来源：http://zq.szsharing.cn

TS:   a && b || !c
来源：http://wh.huixiangedu.cn

Java: a && b || !c
来源：http://ce.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ii.colortex.cn

Ruby: a && b || !c
来源：http://in.yuntaijiaju.cn

C#:   a && b || !c
来源：http://cl.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jn.shxzskj.cn

Py:   if not data: return
来源：http://ii.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://yn.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://nu.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://vm.yuexingan06.cn

Java: if (data == null) return;
来源：http://zl.haigaiapp.cn

Go:   if data == nil { return }
来源：http://um.nicolike.cn

Ruby: return if data.nil?
来源：http://ib.chemitech.net.cn

C#:   if (data == null) return;
来源：http://hx.lnxyls.cn

================================================================================
来源：http://rb.szxytkj.cn

C. 函数与作用域
来源：http://lw.haigaiapp.cn

================================================================================
来源：http://jc.szxytkj.cn

[C01] 定义函数
来源：http://qi.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://tk.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dr.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://mf.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ho.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fp.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rj.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://rr.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kg.bookmarksfly.cn

[C02] 默认参数
来源：http://km.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://tz.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pt.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://ch.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qj.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fk.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kk.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://nb.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://my.huanxung.cn

[C03] 可变参数
来源：http://dp.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://eo.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eg.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ky.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ks.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mc.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jw.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://by.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gh.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://fp.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hj.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qq.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ed.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ci.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ex.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://xa.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://dp.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://gr.wgjwhj.cn

[C05] 返回多个值
来源：http://vq.huixiangedu.cn

Py:   return a, b
来源：http://ct.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ds.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ax.chemitech.net.cn

TS:   return { a, b };
来源：http://gk.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://id.muxihuayi.cn

Go:   return a, b
来源：http://cx.bjjhwx.cn

Ruby: return a, b
来源：http://ja.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://we.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://qf.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ch.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sn.shxzskj.cn

JS:   const square = x => x * x;
来源：http://cr.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://qf.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://me.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dd.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://id.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ks.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://kc.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uw.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wc.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pm.jctech888.com.cn

TS:   arr.map(String)
来源：http://re.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zt.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bj.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://jp.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ym.wgjwhj.cn

[C08] 闭包
来源：http://ru.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kz.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ix.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wc.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dm.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ve.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vv.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ib.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vm.shtwfgs.cn

[C09] 递归
来源：http://ph.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cx.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ah.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lt.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bi.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bp.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hk.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vt.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ng.colortex.cn

[C10] 变量作用域
来源：http://bu.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cz.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rl.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oa.shxzskj.cn

TS:   同 JS
来源：http://vs.nicolike.cn

Java: 方法内为块级作用域
来源：http://ca.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://ka.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dq.wgjwhj.cn

C#:   块级作用域
来源：http://gg.hahajie.cn

[C11] 模块导入与导出
来源：http://oz.yuntaijiaju.cn

Py:   from module import func
来源：http://jn.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://re.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ir.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gs.szsharing.cn

Java: import java.util.List;
来源：http://gj.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dt.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://fx.bjjhwx.cn

C#:   using System.Text;
来源：http://mk.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://or.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://wc.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://bp.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://xl.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://yu.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zd.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://tb.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://qd.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yk.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://fm.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ee.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wj.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xf.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wa.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ru.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ou.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kj.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ed.haigaiapp.cn

[C14] 泛型函数
来源：http://mu.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://po.hahajie.cn

PHP:  // 无泛型
来源：http://vi.wgjwhj.cn

JS:   // 无泛型
来源：http://ym.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cb.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ch.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nv.asd995.cn

Ruby: # 无泛型
来源：http://jb.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ey.521024.cn

[C15] 解构 / 展开参数
来源：http://lv.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nd.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://me.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ie.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cd.nicolike.cn

Java: // 无解构
来源：http://lk.nicolike.cn

Go:   // 无解构
来源：http://yp.huixiangedu.cn

Ruby: a, b = pair
来源：http://sa.nszjky.cn

C#:   var (a, b) = pair;
来源：http://uf.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://eg.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kl.panjiajie.cn

PHP:  // 无重载
来源：http://sq.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pz.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://zu.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rh.521024.cn

Go:   // 无重载：用不同函数名
来源：http://aq.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://ws.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uq.jianghongdianzi.cn

================================================================================
来源：http://rr.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://zj.bookmarksfly.cn

================================================================================
来源：http://bw.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://ud.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ei.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ej.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lh.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cg.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bd.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://fr.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://mq.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wf.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://zg.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yi.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ou.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://od.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://zt.shxzukj.cn

Java: list.add(4);
来源：http://fx.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://pz.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ze.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://pz.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://dx.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://cx.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://us.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xq.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://dl.yuexingan06.cn

Java: list.add(0, 0);
来源：http://hh.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://is.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oy.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://ds.newstarts.cn

[D04] 删除元素
来源：http://kp.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wm.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://el.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ba.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://cy.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wv.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jc.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yl.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nd.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://rt.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gw.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xe.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sh.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://dl.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://gg.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://lx.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gh.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://js.nicolike.cn

[D06] 数组长度
来源：http://fb.colortex.cn

Py:   len(arr)
来源：http://cb.szsharing.cn

PHP:  count($arr);
来源：http://jx.szxytkj.cn

JS:   arr.length
来源：http://tw.haigaiapp.cn

TS:   arr.length
来源：http://ac.colortex.cn

Java: list.size();
来源：http://mq.9csxet.cn

Go:   len(arr)
来源：http://ds.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://vz.shxzskj.cn

C#:   list.Count;
来源：http://mh.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://yv.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lq.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ip.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://wq.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://wy.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://di.bookmarksfly.cn

Go:   arr[1:4]
来源：http://dr.9csxet.cn

Ruby: arr[1, 3]
来源：http://xb.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://jz.bjjhwx.cn

[D08] 合并两个数组
来源：http://hq.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://fa.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://au.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sn.lnxyls.cn

TS:   [...a, ...b];
来源：http://cy.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yr.szxytkj.cn

Go:   append(a, b...)
来源：http://ir.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ea.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://kr.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://iy.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://fd.newstarts.cn

PHP:  sort($arr);
来源：http://uy.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ka.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xo.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xg.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lp.9csxet.cn

Ruby: arr.sort
来源：http://vs.huanxung.cn

C#:   list.Sort();
来源：http://eu.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sh.hnjuh.cn


<!-- 参考信息 -->