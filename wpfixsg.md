代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://el.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iy.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://vj.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://my.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://po.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yp.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gv.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pq.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gf.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://nb.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://he.521024.cn

[B12] 跳出多层循环
来源：http://ae.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://na.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nn.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://st.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kb.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mp.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cf.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dv.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ba.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://zt.lnxyls.cn

PHP:  is_numeric($x)
来源：http://tq.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cj.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fz.huixiangedu.cn

Java: x instanceof Number
来源：http://uh.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://am.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://du.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://yu.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://he.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ou.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kj.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://vk.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ic.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ga.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mp.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ky.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xx.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://pu.nicolike.cn

Py:   a and b or not c
来源：http://ss.asd995.cn

PHP:  $a && $b || !$c
来源：http://jk.shxzukj.cn

JS:   a && b || !c
来源：http://fv.9csxet.cn

TS:   a && b || !c
来源：http://uc.yuexingan06.cn

Java: a && b || !c
来源：http://op.nicolike.cn

Go:   a && b || !c
来源：http://hs.hahajie.cn

Ruby: a && b || !c
来源：http://jr.newstarts.cn

C#:   a && b || !c
来源：http://df.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tq.bjjhwx.cn

Py:   if not data: return
来源：http://mc.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://on.9csxet.cn

JS:   if (!data) return;
来源：http://xr.jctech888.com.cn

TS:   if (!data) return;
来源：http://dm.bjjhwx.cn

Java: if (data == null) return;
来源：http://fp.lnxyls.cn

Go:   if data == nil { return }
来源：http://cc.nszjky.cn

Ruby: return if data.nil?
来源：http://jt.huixiangedu.cn

C#:   if (data == null) return;
来源：http://yn.shtwfgs.cn

================================================================================
来源：http://pb.yuexingan06.cn

C. 函数与作用域
来源：http://pq.shxzskj.cn

================================================================================
来源：http://ql.nszjky.cn

[C01] 定义函数
来源：http://mt.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://qc.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://uw.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nl.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fu.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mw.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://pz.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wp.nszjky.cn

[C02] 默认参数
来源：http://as.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://qw.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ct.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://bc.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ma.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bd.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uj.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ms.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ab.jianghongdianzi.cn

[C03] 可变参数
来源：http://wz.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://xc.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ui.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fv.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pp.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://al.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cc.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fp.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fv.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://wk.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pn.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pa.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vv.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qo.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://xc.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ut.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://dt.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://iv.newstarts.cn

[C05] 返回多个值
来源：http://dc.wgjwhj.cn

Py:   return a, b
来源：http://ex.panjiajie.cn

PHP:  return [$a, $b];
来源：http://xs.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://za.shtwfgs.cn

TS:   return { a, b };
来源：http://xo.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tn.bookmarksfly.cn

Go:   return a, b
来源：http://th.shtwfgs.cn

Ruby: return a, b
来源：http://sd.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://zr.521024.cn

[C06] 匿名函数 / lambda
来源：http://bv.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://qr.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gn.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://lr.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ny.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://md.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wy.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://so.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bw.hahajie.cn

[C07] 把函数作为参数传入
来源：http://ri.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cl.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ut.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xj.lnxyls.cn

TS:   arr.map(String)
来源：http://ax.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xy.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nu.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://nj.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ya.gzmigu.cn

[C08] 闭包
来源：http://kn.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mb.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rb.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kg.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bw.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kj.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mz.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xi.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qa.shxzskj.cn

[C09] 递归
来源：http://ee.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ix.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ut.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uc.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jw.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qe.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wy.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qh.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ja.shtwfgs.cn

[C10] 变量作用域
来源：http://cn.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://at.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zq.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dt.nszjky.cn

TS:   同 JS
来源：http://wj.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://fz.521024.cn

Go:   花括号块级作用域
来源：http://ku.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yk.shxzskj.cn

C#:   块级作用域
来源：http://nz.asd995.cn

[C11] 模块导入与导出
来源：http://rl.huixiangedu.cn

Py:   from module import func
来源：http://il.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fh.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ri.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mi.shxzskj.cn

Java: import java.util.List;
来源：http://tr.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bf.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://xx.jctech888.com.cn

C#:   using System.Text;
来源：http://hi.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://zc.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://fa.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://qi.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://hp.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://qo.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lf.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://dh.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://uj.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zr.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://tv.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rq.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lp.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pj.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rg.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xe.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://wm.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ab.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nf.huixiangedu.cn

[C14] 泛型函数
来源：http://kw.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xs.szsharing.cn

PHP:  // 无泛型
来源：http://tq.yuntaijiaju.cn

JS:   // 无泛型
来源：http://tk.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kr.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://re.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iz.huanxung.cn

Ruby: # 无泛型
来源：http://kb.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ic.nszjky.cn

[C15] 解构 / 展开参数
来源：http://pu.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yd.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://qn.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hp.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ec.asd995.cn

Java: // 无解构
来源：http://qj.gzmigu.cn

Go:   // 无解构
来源：http://rf.yuexingan06.cn

Ruby: a, b = pair
来源：http://es.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ix.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://dq.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qv.lnxyls.cn

PHP:  // 无重载
来源：http://sv.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nl.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://xu.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yq.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://tt.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://vj.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xw.shxzskj.cn

================================================================================
来源：http://tn.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://wk.shxzskj.cn

================================================================================
来源：http://xj.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://ek.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gf.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yp.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rs.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gt.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gg.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ue.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://iq.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wm.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://hw.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tu.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://do.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://qi.bjjhwx.cn

TS:   arr.push(4);
来源：http://oo.gzmigu.cn

Java: list.add(4);
来源：http://rk.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://wt.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ob.chemitech.net.cn

C#:   list.Add(4);
来源：http://mk.huanxung.cn

[D03] 在指定位置插入元素
来源：http://qh.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ke.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://by.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lv.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://dn.szsharing.cn

Java: list.add(0, 0);
来源：http://wh.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yu.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xp.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://mj.huanxung.cn

[D04] 删除元素
来源：http://wt.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uy.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uj.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iw.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ip.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hr.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gt.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ew.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uj.gzmigu.cn

[D05] 访问与修改元素
来源：http://ap.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uh.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ay.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://sn.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://kj.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ui.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wd.521024.cn

[D06] 数组长度
来源：http://zp.gzmigu.cn

Py:   len(arr)
来源：http://tn.lnxyls.cn

PHP:  count($arr);
来源：http://yw.chemitech.net.cn

JS:   arr.length
来源：http://gg.gzmigu.cn

TS:   arr.length
来源：http://mf.hnjuh.cn

Java: list.size();
来源：http://qm.yuexingan06.cn

Go:   len(arr)
来源：http://gk.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://ps.chemitech.net.cn

C#:   list.Count;
来源：http://qo.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ic.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jl.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mt.colortex.cn

JS:   arr.slice(1, 4);
来源：http://sh.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://dx.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://hx.nicolike.cn

Go:   arr[1:4]
来源：http://cm.shxzukj.cn

Ruby: arr[1, 3]
来源：http://aq.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://pr.huixiangedu.cn

[D08] 合并两个数组
来源：http://ez.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://eq.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://yk.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://la.haigaiapp.cn

TS:   [...a, ...b];
来源：http://rh.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xu.newstarts.cn

Go:   append(a, b...)
来源：http://wb.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://lc.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://fj.newstarts.cn

[D09] 排序（升序）
来源：http://jm.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ke.bookmarksfly.cn

PHP:  sort($arr);
来源：http://xx.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uc.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lq.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gw.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ph.jctech888.com.cn

Ruby: arr.sort
来源：http://xp.szsharing.cn

C#:   list.Sort();
来源：http://jh.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mp.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://na.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wl.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rt.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ph.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://id.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ks.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mk.szsharing.cn

[D11] 反转数组
来源：http://sm.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ds.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://gn.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ah.bookmarksfly.cn


<!-- 参考信息 -->