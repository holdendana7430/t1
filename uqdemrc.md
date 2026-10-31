代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wi.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mm.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://my.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://rl.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://um.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xu.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zp.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://js.colortex.cn

[B09] break 与 continue
来源：http://jp.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ux.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://il.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fb.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hj.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xm.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pz.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ic.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eg.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://es.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qx.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ub.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cu.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zk.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zi.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://te.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://ix.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://bo.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://qw.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wc.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mm.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lj.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://hu.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://un.huanxung.cn

[B12] 跳出多层循环
来源：http://ck.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://in.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zn.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pq.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bn.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://se.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ku.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ky.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dc.yuexingan06.cn

[B13] 判断是否为数字
来源：http://xq.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://cr.panjiajie.cn

PHP:  is_numeric($x)
来源：http://ky.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pe.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hi.bookmarksfly.cn

Java: x instanceof Number
来源：http://nx.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://li.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://zy.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://iq.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://au.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hd.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kz.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://in.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://xh.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://db.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://of.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wq.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zf.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://va.shxzukj.cn

Py:   a and b or not c
来源：http://dy.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://sc.wgjwhj.cn

JS:   a && b || !c
来源：http://gl.huixiangedu.cn

TS:   a && b || !c
来源：http://mg.nszjky.cn

Java: a && b || !c
来源：http://zk.yuexingan06.cn

Go:   a && b || !c
来源：http://ir.huixiangedu.cn

Ruby: a && b || !c
来源：http://zc.bookmarksfly.cn

C#:   a && b || !c
来源：http://wu.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iw.wgjwhj.cn

Py:   if not data: return
来源：http://rm.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://bl.huixiangedu.cn

JS:   if (!data) return;
来源：http://kl.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://js.colortex.cn

Java: if (data == null) return;
来源：http://ql.wgjwhj.cn

Go:   if data == nil { return }
来源：http://zq.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://kp.newstarts.cn

C#:   if (data == null) return;
来源：http://uv.yuexingan06.cn

================================================================================
来源：http://tu.hnjuh.cn

C. 函数与作用域
来源：http://wm.huixiangedu.cn

================================================================================
来源：http://if.hnjuh.cn

[C01] 定义函数
来源：http://ym.521024.cn

Py:   def add(a, b): return a + b
来源：http://er.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ox.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://gk.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ix.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kt.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://mf.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xe.huixinmuqiang.cn

[C02] 默认参数
来源：http://et.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://cr.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wp.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://yq.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oq.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qy.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cu.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ql.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://xk.nszjky.cn

[C03] 可变参数
来源：http://za.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://zi.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vu.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pm.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://np.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bo.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zg.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jq.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xt.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://qj.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tb.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cd.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://us.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zc.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://eg.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://uz.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://qs.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://vx.bjjhwx.cn

[C05] 返回多个值
来源：http://pt.panjiajie.cn

Py:   return a, b
来源：http://rh.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://vm.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ux.muxihuayi.cn

TS:   return { a, b };
来源：http://lz.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cb.chemitech.net.cn

Go:   return a, b
来源：http://vn.hahajie.cn

Ruby: return a, b
来源：http://fz.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://mk.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pi.newstarts.cn

Py:   square = lambda x: x * x
来源：http://lg.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xh.asd995.cn

JS:   const square = x => x * x;
来源：http://tn.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://eh.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dw.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dh.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://ls.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hm.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://bb.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yh.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ez.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://th.huanxung.cn

TS:   arr.map(String)
来源：http://ng.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xw.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ly.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ce.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ut.bjjhwx.cn

[C08] 闭包
来源：http://js.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://or.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wv.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://de.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ke.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hk.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://go.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tw.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nj.colortex.cn

[C09] 递归
来源：http://ql.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qp.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mi.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://do.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yq.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sw.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zb.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bd.wgjwhj.cn

[C10] 变量作用域
来源：http://ph.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yp.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ht.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gu.nicolike.cn

TS:   同 JS
来源：http://od.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://iy.lnxyls.cn

Go:   花括号块级作用域
来源：http://ed.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tl.shxzskj.cn

C#:   块级作用域
来源：http://hl.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://hf.hahajie.cn

Py:   from module import func
来源：http://cz.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jq.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kr.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lq.wgjwhj.cn

Java: import java.util.List;
来源：http://id.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ct.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://nd.jctech888.com.cn

C#:   using System.Text;
来源：http://al.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://lc.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://pb.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://aa.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://fk.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://xb.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mv.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://vo.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://nw.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://se.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://qz.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zd.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pn.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mn.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qr.shxzukj.cn

Go:   func add(a, b int) int
来源：http://yu.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kj.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oi.hnjuh.cn

[C14] 泛型函数
来源：http://zh.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fv.nszjky.cn

PHP:  // 无泛型
来源：http://kk.huanxung.cn

JS:   // 无泛型
来源：http://fo.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ua.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kl.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mi.szxytkj.cn

Ruby: # 无泛型
来源：http://bv.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://on.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://so.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eg.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://og.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ft.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vg.hahajie.cn

Java: // 无解构
来源：http://hf.shtwfgs.cn

Go:   // 无解构
来源：http://sv.hahajie.cn

Ruby: a, b = pair
来源：http://vx.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ek.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ve.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ho.shxzukj.cn

PHP:  // 无重载
来源：http://qz.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rb.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://fc.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ud.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://ji.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://lt.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zg.hahajie.cn

================================================================================
来源：http://ja.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://qa.colortex.cn

================================================================================
来源：http://ht.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://wp.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mm.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sa.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tx.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vo.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ud.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://gh.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://bv.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ae.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://re.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rn.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ei.jctech888.com.cn

JS:   arr.push(4);
来源：http://om.muxihuayi.cn

TS:   arr.push(4);
来源：http://tl.521024.cn

Java: list.add(4);
来源：http://mx.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://au.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://zz.521024.cn

C#:   list.Add(4);
来源：http://qn.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://ui.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://bj.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fz.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://os.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://qm.panjiajie.cn

Java: list.add(0, 0);
来源：http://mg.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bx.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sl.asd995.cn

C#:   list.Insert(0, 0);
来源：http://yr.szxytkj.cn

[D04] 删除元素
来源：http://dv.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mt.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vd.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fa.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://nr.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bi.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wi.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kp.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kh.szxytkj.cn

[D05] 访问与修改元素
来源：http://nx.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tb.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ap.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bb.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://oy.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://uu.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://ng.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iu.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uw.muxihuayi.cn

[D06] 数组长度
来源：http://eh.shtwfgs.cn

Py:   len(arr)
来源：http://ce.yuexingan06.cn

PHP:  count($arr);
来源：http://zm.bookmarksfly.cn

JS:   arr.length
来源：http://zw.bjjhwx.cn

TS:   arr.length
来源：http://pf.shxzskj.cn

Java: list.size();
来源：http://tk.shtwfgs.cn

Go:   len(arr)
来源：http://ve.asd995.cn

Ruby: arr.length; arr.size
来源：http://ym.panjiajie.cn

C#:   list.Count;
来源：http://mi.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://ht.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cf.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fm.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://me.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://nz.9csxet.cn

Java: list.subList(1, 4);
来源：http://br.haigaiapp.cn

Go:   arr[1:4]
来源：http://lz.gzmigu.cn

Ruby: arr[1, 3]
来源：http://ua.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://vo.nicolike.cn

[D08] 合并两个数组
来源：http://gy.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://oa.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://et.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mq.yuexingan06.cn

TS:   [...a, ...b];
来源：http://ax.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ny.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://wh.yuntaijiaju.cn


<!-- 参考信息 -->