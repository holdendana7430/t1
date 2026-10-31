代发 wailian999

C#:   x is int or double or decimal
来源：http://ar.szsharing.cn

[B14] 判断值是否在集合内
来源：http://vk.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aw.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://np.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://wv.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://uj.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fw.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oy.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mg.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nz.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ct.nicolike.cn

Py:   a and b or not c
来源：http://fo.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://vc.wgjwhj.cn

JS:   a && b || !c
来源：http://lp.hahajie.cn

TS:   a && b || !c
来源：http://xi.muxihuayi.cn

Java: a && b || !c
来源：http://tq.haigaiapp.cn

Go:   a && b || !c
来源：http://ex.shxzukj.cn

Ruby: a && b || !c
来源：http://wv.bookmarksfly.cn

C#:   a && b || !c
来源：http://zu.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oe.9csxet.cn

Py:   if not data: return
来源：http://qg.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ql.9csxet.cn

JS:   if (!data) return;
来源：http://ja.nicolike.cn

TS:   if (!data) return;
来源：http://ay.huanxung.cn

Java: if (data == null) return;
来源：http://pn.wgjwhj.cn

Go:   if data == nil { return }
来源：http://th.hahajie.cn

Ruby: return if data.nil?
来源：http://od.huanxung.cn

C#:   if (data == null) return;
来源：http://gr.shtwfgs.cn

================================================================================
来源：http://ni.yuexingan06.cn

C. 函数与作用域
来源：http://rj.huixiangedu.cn

================================================================================
来源：http://im.yuexingan06.cn

[C01] 定义函数
来源：http://uv.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://if.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xy.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://fx.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ys.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wt.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zi.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://nu.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vs.yuntaijiaju.cn

[C02] 默认参数
来源：http://ay.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://nd.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ae.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://ai.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cy.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wo.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fc.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://qc.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://qc.yuexingan06.cn

[C03] 可变参数
来源：http://vs.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://yd.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mx.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ze.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://to.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yf.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lz.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://da.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zh.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://nz.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sp.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ub.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vp.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sv.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://gr.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://xr.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://ln.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ml.bookmarksfly.cn

[C05] 返回多个值
来源：http://ar.yuexingan06.cn

Py:   return a, b
来源：http://wy.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://ol.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ct.colortex.cn

TS:   return { a, b };
来源：http://df.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sy.szxytkj.cn

Go:   return a, b
来源：http://wq.lnxyls.cn

Ruby: return a, b
来源：http://ux.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://ic.521024.cn

[C06] 匿名函数 / lambda
来源：http://xt.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://qc.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kk.521024.cn

JS:   const square = x => x * x;
来源：http://qc.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://nc.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yn.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jr.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://as.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jl.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://cz.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wc.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fy.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xg.asd995.cn

TS:   arr.map(String)
来源：http://pg.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ll.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://an.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://ru.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://os.hnjuh.cn

[C08] 闭包
来源：http://hd.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zw.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xl.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nv.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nh.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nk.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xg.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://op.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xf.yuntaijiaju.cn

[C09] 递归
来源：http://ti.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jn.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jg.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yf.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hb.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wj.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zc.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://av.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://az.huixinmuqiang.cn

[C10] 变量作用域
来源：http://pi.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zk.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bk.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uh.huixiangedu.cn

TS:   同 JS
来源：http://rv.huanxung.cn

Java: 方法内为块级作用域
来源：http://vo.szxytkj.cn

Go:   花括号块级作用域
来源：http://dx.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ns.yuexingan06.cn

C#:   块级作用域
来源：http://eo.jctech888.com.cn

[C11] 模块导入与导出
来源：http://oc.huixinmuqiang.cn

Py:   from module import func
来源：http://qf.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ci.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nj.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mx.lnxyls.cn

Java: import java.util.List;
来源：http://ap.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kn.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ok.nicolike.cn

C#:   using System.Text;
来源：http://cq.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://lk.521024.cn

Py:   (lambda: print("run"))()
来源：http://of.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://sp.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://rr.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://fk.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qf.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://dg.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://fv.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://in.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://fe.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sx.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lc.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://et.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qf.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cz.huanxung.cn

Go:   func add(a, b int) int
来源：http://be.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ht.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nz.shtwfgs.cn

[C14] 泛型函数
来源：http://ia.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cc.huanxung.cn

PHP:  // 无泛型
来源：http://sd.huanxung.cn

JS:   // 无泛型
来源：http://pz.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yw.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gk.szsharing.cn

Ruby: # 无泛型
来源：http://xz.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ej.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://hy.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cw.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://ef.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rg.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hh.nicolike.cn

Java: // 无解构
来源：http://sw.yuntaijiaju.cn

Go:   // 无解构
来源：http://ls.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://cr.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://js.asd995.cn

[C16] 函数 / 方法重载
来源：http://bg.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kz.521024.cn

PHP:  // 无重载
来源：http://im.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fo.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://wj.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lp.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://qi.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://am.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://be.jianghongdianzi.cn

================================================================================
来源：http://wq.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://qn.szsharing.cn

================================================================================
来源：http://xh.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://xi.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cu.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qq.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sd.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ed.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yj.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://jd.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ov.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vy.9csxet.cn

[D02] 追加元素到末尾
来源：http://us.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ye.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ir.shxzskj.cn

JS:   arr.push(4);
来源：http://am.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://bx.gzmigu.cn

Java: list.add(4);
来源：http://lj.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://tg.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://hv.bookmarksfly.cn

C#:   list.Add(4);
来源：http://go.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://bv.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://kt.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xl.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eb.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://rv.hnjuh.cn

Java: list.add(0, 0);
来源：http://gp.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xu.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mm.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ej.jctech888.com.cn

[D04] 删除元素
来源：http://kp.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dx.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vm.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://su.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://si.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ka.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wz.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bu.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hc.9csxet.cn

[D05] 访问与修改元素
来源：http://lj.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pk.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pz.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uw.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://pf.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://vn.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://rq.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xi.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wv.newstarts.cn

[D06] 数组长度
来源：http://ex.nszjky.cn

Py:   len(arr)
来源：http://ua.szxytkj.cn

PHP:  count($arr);
来源：http://po.szxytkj.cn

JS:   arr.length
来源：http://cs.hahajie.cn

TS:   arr.length
来源：http://oq.colortex.cn

Java: list.size();
来源：http://jp.haigaiapp.cn

Go:   len(arr)
来源：http://wd.9csxet.cn

Ruby: arr.length; arr.size
来源：http://bo.shxzukj.cn

C#:   list.Count;
来源：http://fo.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ug.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://an.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mh.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://za.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://nr.nszjky.cn

Java: list.subList(1, 4);
来源：http://qn.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://hw.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://zm.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://zp.shtwfgs.cn

[D08] 合并两个数组
来源：http://vq.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://lg.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://jq.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tg.szxytkj.cn

TS:   [...a, ...b];
来源：http://dt.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nu.haigaiapp.cn

Go:   append(a, b...)
来源：http://tw.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ni.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://qo.huanxung.cn

[D09] 排序（升序）
来源：http://em.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://lu.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gr.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dw.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tf.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ty.9csxet.cn

Ruby: arr.sort
来源：http://mx.shxzukj.cn

C#:   list.Sort();
来源：http://lg.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wz.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nt.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vw.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sv.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kw.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xj.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tu.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ef.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tf.chemitech.net.cn

[D11] 反转数组
来源：http://ng.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://om.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://dg.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zg.hahajie.cn

TS:   [...arr].reverse();
来源：http://xe.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://bh.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://pu.colortex.cn

Ruby: arr.reverse
来源：http://yd.chemitech.net.cn

C#:   list.Reverse();
来源：http://bx.szxytkj.cn

[D12] 查找元素下标
来源：http://je.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://fc.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ia.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pm.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ca.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hq.colortex.cn

Go:   slices.Index(arr, x)
来源：http://xx.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ca.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://lx.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://gu.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qp.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bs.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://ks.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://xd.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dl.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tt.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vz.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yp.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://bv.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gk.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xg.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ev.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://xs.shxzskj.cn


<!-- 参考信息 -->