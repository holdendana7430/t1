代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pp.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://qy.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jj.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://de.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jv.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dq.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zp.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sg.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://za.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rv.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ht.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://rf.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://er.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ue.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ti.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hy.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://np.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://vy.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oz.yuexingan06.cn

[B12] 跳出多层循环
来源：http://hr.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rt.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fr.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wf.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ce.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nn.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ab.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fx.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://me.yuexingan06.cn

[B13] 判断是否为数字
来源：http://vf.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://oe.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ru.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pe.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tu.lnxyls.cn

Java: x instanceof Number
来源：http://at.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lc.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ol.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ax.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://dg.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kr.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dy.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://ov.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ik.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zh.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iw.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zb.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://af.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://tt.jianghongdianzi.cn

Py:   a and b or not c
来源：http://ul.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://gv.nicolike.cn

JS:   a && b || !c
来源：http://rf.hnjuh.cn

TS:   a && b || !c
来源：http://yg.nszjky.cn

Java: a && b || !c
来源：http://tl.haigaiapp.cn

Go:   a && b || !c
来源：http://av.521024.cn

Ruby: a && b || !c
来源：http://np.yuntaijiaju.cn

C#:   a && b || !c
来源：http://fr.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ri.szsharing.cn

Py:   if not data: return
来源：http://pd.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://yc.wgjwhj.cn

JS:   if (!data) return;
来源：http://fa.asd995.cn

TS:   if (!data) return;
来源：http://it.haigaiapp.cn

Java: if (data == null) return;
来源：http://xx.wgjwhj.cn

Go:   if data == nil { return }
来源：http://wo.muxihuayi.cn

Ruby: return if data.nil?
来源：http://ik.huixiangedu.cn

C#:   if (data == null) return;
来源：http://zr.nicolike.cn

================================================================================
来源：http://do.huixinmuqiang.cn

C. 函数与作用域
来源：http://de.chemitech.net.cn

================================================================================
来源：http://gy.newstarts.cn

[C01] 定义函数
来源：http://hc.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://qi.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ts.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://qc.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ps.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yl.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cn.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://na.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ir.shxzukj.cn

[C02] 默认参数
来源：http://oi.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://al.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zg.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://zt.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fq.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hc.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ra.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://nw.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://sm.jctech888.com.cn

[C03] 可变参数
来源：http://kr.521024.cn

Py:   def total(*args): return sum(args)
来源：http://fv.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fl.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fe.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gj.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aj.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hk.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cd.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oa.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ud.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xb.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ae.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sx.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lu.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://es.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://dl.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://bo.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ch.bookmarksfly.cn

[C05] 返回多个值
来源：http://on.yuntaijiaju.cn

Py:   return a, b
来源：http://ln.panjiajie.cn

PHP:  return [$a, $b];
来源：http://lq.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kq.shxzskj.cn

TS:   return { a, b };
来源：http://zb.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ue.haigaiapp.cn

Go:   return a, b
来源：http://jy.yuexingan06.cn

Ruby: return a, b
来源：http://sc.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xw.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://cc.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://hb.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vs.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://bz.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://wz.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kp.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vs.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://kl.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ww.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://am.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ja.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yl.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rp.bookmarksfly.cn

TS:   arr.map(String)
来源：http://qy.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nz.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ct.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ce.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kv.bookmarksfly.cn

[C08] 闭包
来源：http://il.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xw.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dw.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uo.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cl.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tw.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xe.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wu.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://is.haigaiapp.cn

[C09] 递归
来源：http://nq.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://of.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ua.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vy.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ys.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zb.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jz.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jt.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aq.szxytkj.cn

[C10] 变量作用域
来源：http://ka.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ta.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lp.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eq.shxzskj.cn

TS:   同 JS
来源：http://wg.colortex.cn

Java: 方法内为块级作用域
来源：http://hs.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://og.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tk.bookmarksfly.cn

C#:   块级作用域
来源：http://zk.huanxung.cn

[C11] 模块导入与导出
来源：http://re.chemitech.net.cn

Py:   from module import func
来源：http://tw.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gd.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hi.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://za.bookmarksfly.cn

Java: import java.util.List;
来源：http://lp.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lh.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ut.haigaiapp.cn

C#:   using System.Text;
来源：http://va.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://vd.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://av.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ri.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ak.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ez.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gv.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://qw.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://te.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ve.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ut.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tf.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qt.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ck.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ll.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yz.szxytkj.cn

Go:   func add(a, b int) int
来源：http://vj.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iy.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kw.lnxyls.cn

[C14] 泛型函数
来源：http://mf.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sh.bjjhwx.cn

PHP:  // 无泛型
来源：http://ld.huixiangedu.cn

JS:   // 无泛型
来源：http://zo.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xy.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zo.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://av.asd995.cn

Ruby: # 无泛型
来源：http://zu.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rr.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://bz.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kp.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://jv.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://od.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pz.muxihuayi.cn

Java: // 无解构
来源：http://nv.asd995.cn

Go:   // 无解构
来源：http://oj.nicolike.cn

Ruby: a, b = pair
来源：http://fu.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://pa.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://tt.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wo.lnxyls.cn

PHP:  // 无重载
来源：http://rw.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://io.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://jl.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kb.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ef.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ux.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qg.szxytkj.cn

================================================================================
来源：http://xj.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ln.newstarts.cn

================================================================================
来源：http://rq.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://ai.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ku.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qv.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wo.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fb.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zx.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://el.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://sp.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ed.newstarts.cn

[D02] 追加元素到末尾
来源：http://tq.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pt.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ik.szsharing.cn

JS:   arr.push(4);
来源：http://qc.shtwfgs.cn

TS:   arr.push(4);
来源：http://ng.muxihuayi.cn

Java: list.add(4);
来源：http://mt.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://xh.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://uv.jctech888.com.cn

C#:   list.Add(4);
来源：http://dd.nicolike.cn

[D03] 在指定位置插入元素
来源：http://gh.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://ze.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ro.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yr.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ro.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rf.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://di.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://dp.shxzskj.cn

[D04] 删除元素
来源：http://fx.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ps.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qt.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tz.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://qx.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ah.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sr.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bu.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yy.nicolike.cn

[D05] 访问与修改元素
来源：http://bm.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ro.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pl.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://av.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://uj.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yh.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://mc.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ty.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xx.shtwfgs.cn

[D06] 数组长度
来源：http://op.hnjuh.cn

Py:   len(arr)
来源：http://ps.yuexingan06.cn

PHP:  count($arr);
来源：http://uw.jianghongdianzi.cn

JS:   arr.length
来源：http://oc.huixinmuqiang.cn

TS:   arr.length
来源：http://fd.huixiangedu.cn

Java: list.size();
来源：http://pv.colortex.cn

Go:   len(arr)
来源：http://jk.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://kl.jctech888.com.cn

C#:   list.Count;
来源：http://gf.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://ev.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mh.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://im.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://ov.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://nq.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ns.asd995.cn

Go:   arr[1:4]
来源：http://uh.szxytkj.cn

Ruby: arr[1, 3]
来源：http://on.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://js.bjjhwx.cn

[D08] 合并两个数组
来源：http://jr.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://fm.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ya.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://op.asd995.cn

TS:   [...a, ...b];
来源：http://ro.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eb.huanxung.cn

Go:   append(a, b...)
来源：http://na.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://kk.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://xl.gzmigu.cn

[D09] 排序（升序）
来源：http://sl.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qc.asd995.cn

PHP:  sort($arr);
来源：http://mh.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eu.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yi.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mw.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tb.hahajie.cn

Ruby: arr.sort
来源：http://rx.panjiajie.cn

C#:   list.Sort();
来源：http://im.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://et.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kq.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zg.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ms.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nv.huixiangedu.cn


<!-- 参考信息 -->