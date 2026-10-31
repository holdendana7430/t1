代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://at.yuexingan06.cn

Java: x instanceof Number
来源：http://vk.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zo.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://fg.521024.cn

C#:   x is int or double or decimal
来源：http://uz.huanxung.cn

[B14] 判断值是否在集合内
来源：http://gx.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jr.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jw.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://qy.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://ch.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ad.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://he.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ln.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dx.nszjky.cn

[B15] 布尔运算与取反
来源：http://cg.shxzskj.cn

Py:   a and b or not c
来源：http://hg.nszjky.cn

PHP:  $a && $b || !$c
来源：http://bp.colortex.cn

JS:   a && b || !c
来源：http://sv.huixinmuqiang.cn

TS:   a && b || !c
来源：http://to.szxytkj.cn

Java: a && b || !c
来源：http://lh.lnxyls.cn

Go:   a && b || !c
来源：http://fp.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ih.bjjhwx.cn

C#:   a && b || !c
来源：http://ss.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vp.szxytkj.cn

Py:   if not data: return
来源：http://yx.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://ng.hnjuh.cn

JS:   if (!data) return;
来源：http://pi.chemitech.net.cn

TS:   if (!data) return;
来源：http://mq.bookmarksfly.cn

Java: if (data == null) return;
来源：http://mr.shtwfgs.cn

Go:   if data == nil { return }
来源：http://gs.521024.cn

Ruby: return if data.nil?
来源：http://qa.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ww.lnxyls.cn

================================================================================
来源：http://hj.colortex.cn

C. 函数与作用域
来源：http://lk.chemitech.net.cn

================================================================================
来源：http://zb.shxzukj.cn

[C01] 定义函数
来源：http://bu.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://sn.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zk.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://wd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oa.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zo.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jt.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://dr.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jp.shxzukj.cn

[C02] 默认参数
来源：http://rl.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://st.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wk.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://es.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ub.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ki.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ct.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ju.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://aj.huanxung.cn

[C03] 可变参数
来源：http://ng.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://hn.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ni.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zz.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kc.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ah.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fy.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ux.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://js.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://os.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tz.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://us.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rt.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ub.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ru.521024.cn

Go:   // 无：用配置结构体参数
来源：http://oy.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://td.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://ib.bookmarksfly.cn

[C05] 返回多个值
来源：http://ss.shxzskj.cn

Py:   return a, b
来源：http://re.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://yw.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://at.asd995.cn

TS:   return { a, b };
来源：http://io.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fb.bookmarksfly.cn

Go:   return a, b
来源：http://tl.chemitech.net.cn

Ruby: return a, b
来源：http://cv.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ll.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://xf.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://xc.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fx.nicolike.cn

JS:   const square = x => x * x;
来源：http://xr.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://eu.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jr.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://do.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://uv.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://od.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://fa.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jv.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vm.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hq.haigaiapp.cn

TS:   arr.map(String)
来源：http://se.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vb.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tx.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://tp.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ev.szsharing.cn

[C08] 闭包
来源：http://fo.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nf.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jd.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ps.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xe.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aq.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qy.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ku.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ve.9csxet.cn

[C09] 递归
来源：http://hj.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zx.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tw.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://es.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hm.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dg.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eb.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oh.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sj.yuntaijiaju.cn

[C10] 变量作用域
来源：http://vd.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ks.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rd.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ie.nicolike.cn

TS:   同 JS
来源：http://kp.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://od.gzmigu.cn

Go:   花括号块级作用域
来源：http://gp.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zp.lnxyls.cn

C#:   块级作用域
来源：http://is.nszjky.cn

[C11] 模块导入与导出
来源：http://gb.9csxet.cn

Py:   from module import func
来源：http://sh.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ca.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://je.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pv.nicolike.cn

Java: import java.util.List;
来源：http://cj.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vm.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://km.9csxet.cn

C#:   using System.Text;
来源：http://af.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://dr.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://yt.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://yt.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://hh.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://eh.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hn.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://sa.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://qy.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lr.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://uf.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gh.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pp.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ry.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pm.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://du.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://iq.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://st.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pn.huanxung.cn

[C14] 泛型函数
来源：http://qa.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ge.nszjky.cn

PHP:  // 无泛型
来源：http://xm.haigaiapp.cn

JS:   // 无泛型
来源：http://ik.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ul.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uf.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ep.colortex.cn

Ruby: # 无泛型
来源：http://gc.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fx.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://ny.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ve.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://ys.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oo.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cf.shxzukj.cn

Java: // 无解构
来源：http://ub.hahajie.cn

Go:   // 无解构
来源：http://xi.asd995.cn

Ruby: a, b = pair
来源：http://mm.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://td.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://ap.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ra.haigaiapp.cn

PHP:  // 无重载
来源：http://xl.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mc.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ba.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ij.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://sm.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://nh.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hy.szxytkj.cn

================================================================================
来源：http://vt.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://sz.colortex.cn

================================================================================
来源：http://lg.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://iv.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jl.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ct.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vq.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://np.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://au.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://ej.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://cm.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qp.lnxyls.cn

[D02] 追加元素到末尾
来源：http://jr.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ma.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dj.huanxung.cn

JS:   arr.push(4);
来源：http://yz.huanxung.cn

TS:   arr.push(4);
来源：http://la.bookmarksfly.cn

Java: list.add(4);
来源：http://zl.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://az.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://tf.panjiajie.cn

C#:   list.Add(4);
来源：http://el.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://wx.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://cn.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mj.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wr.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://vh.nicolike.cn

Java: list.add(0, 0);
来源：http://tj.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kq.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xw.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://ki.yuexingan06.cn

[D04] 删除元素
来源：http://dy.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lp.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zv.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ds.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://hi.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ny.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xx.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zf.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wa.wgjwhj.cn

[D05] 访问与修改元素
来源：http://vr.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tt.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zu.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fq.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://tp.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ib.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://eq.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fs.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ld.wgjwhj.cn

[D06] 数组长度
来源：http://rw.newstarts.cn

Py:   len(arr)
来源：http://cs.jctech888.com.cn

PHP:  count($arr);
来源：http://nf.9csxet.cn

JS:   arr.length
来源：http://dy.yuexingan06.cn

TS:   arr.length
来源：http://yf.hahajie.cn

Java: list.size();
来源：http://bu.yuexingan06.cn

Go:   len(arr)
来源：http://rb.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://rl.nicolike.cn

C#:   list.Count;
来源：http://po.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://eq.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cs.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sn.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://pq.521024.cn

TS:   arr.slice(1, 4);
来源：http://uj.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://af.wgjwhj.cn

Go:   arr[1:4]
来源：http://hf.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zs.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://iq.newstarts.cn

[D08] 合并两个数组
来源：http://oh.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://bz.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://cp.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tk.lnxyls.cn

TS:   [...a, ...b];
来源：http://in.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mv.panjiajie.cn

Go:   append(a, b...)
来源：http://qn.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://yq.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://dy.szxytkj.cn

[D09] 排序（升序）
来源：http://ko.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://au.jctech888.com.cn

PHP:  sort($arr);
来源：http://ov.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kc.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vo.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gn.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cw.szsharing.cn

Ruby: arr.sort
来源：http://wn.shtwfgs.cn

C#:   list.Sort();
来源：http://ye.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tr.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dj.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sx.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ts.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mj.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bd.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uh.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://op.jianghongdianzi.cn

[D11] 反转数组
来源：http://kg.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oo.colortex.cn

PHP:  array_reverse($arr);
来源：http://vi.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ud.newstarts.cn

TS:   [...arr].reverse();
来源：http://hi.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://pk.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://el.szxytkj.cn

Ruby: arr.reverse
来源：http://it.yuexingan06.cn

C#:   list.Reverse();
来源：http://pr.szsharing.cn

[D12] 查找元素下标
来源：http://cj.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://bo.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gn.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zs.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lg.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ws.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://rl.colortex.cn

Ruby: arr.index(x)
来源：http://pe.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://pd.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://oc.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fi.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aj.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://qs.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://bz.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ew.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kx.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bu.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fq.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ez.yuexingan06.cn


<!-- 参考信息 -->