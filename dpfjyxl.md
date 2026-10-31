代发 wailian999

Go:   a && b || !c
来源：http://kq.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ht.lnxyls.cn

C#:   a && b || !c
来源：http://ic.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tm.shxzskj.cn

Py:   if not data: return
来源：http://ac.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://mt.hahajie.cn

JS:   if (!data) return;
来源：http://ar.asd995.cn

TS:   if (!data) return;
来源：http://jg.muxihuayi.cn

Java: if (data == null) return;
来源：http://gc.nicolike.cn

Go:   if data == nil { return }
来源：http://uu.wgjwhj.cn

Ruby: return if data.nil?
来源：http://sn.jctech888.com.cn

C#:   if (data == null) return;
来源：http://gg.bjjhwx.cn

================================================================================
来源：http://nv.bjjhwx.cn

C. 函数与作用域
来源：http://qd.shtwfgs.cn

================================================================================
来源：http://tc.shxzukj.cn

[C01] 定义函数
来源：http://mb.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://wm.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://qm.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lf.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dv.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xp.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://us.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xo.shxzukj.cn

[C02] 默认参数
来源：http://mr.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://rk.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mv.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://kh.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zq.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ek.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://na.521024.cn

Ruby: def greet(name = "World") = name
来源：http://dr.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://cm.yuntaijiaju.cn

[C03] 可变参数
来源：http://wt.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://yy.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rk.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://px.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bp.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tn.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ev.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wz.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://to.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://yj.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dc.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qd.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pl.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pn.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://sm.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://jc.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://at.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://ii.shtwfgs.cn

[C05] 返回多个值
来源：http://cg.yuntaijiaju.cn

Py:   return a, b
来源：http://cs.asd995.cn

PHP:  return [$a, $b];
来源：http://hf.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aw.szxytkj.cn

TS:   return { a, b };
来源：http://fs.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hn.shxzskj.cn

Go:   return a, b
来源：http://xq.huixinmuqiang.cn

Ruby: return a, b
来源：http://hw.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://kr.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://qj.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://rq.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sg.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://ay.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://gy.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tk.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yl.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://rl.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zi.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://ni.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yw.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mj.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ql.jctech888.com.cn

TS:   arr.map(String)
来源：http://qj.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://re.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sj.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://lx.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nw.shxzskj.cn

[C08] 闭包
来源：http://rk.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ga.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yq.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bq.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://st.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://th.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://of.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pe.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zj.chemitech.net.cn

[C09] 递归
来源：http://um.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qc.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ui.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ah.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qi.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zk.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ab.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iz.nszjky.cn

[C10] 变量作用域
来源：http://js.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ih.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ok.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pl.jctech888.com.cn

TS:   同 JS
来源：http://jh.newstarts.cn

Java: 方法内为块级作用域
来源：http://oo.colortex.cn

Go:   花括号块级作用域
来源：http://ow.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ge.huanxung.cn

C#:   块级作用域
来源：http://gh.shxzukj.cn

[C11] 模块导入与导出
来源：http://qu.shtwfgs.cn

Py:   from module import func
来源：http://ml.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xk.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aj.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sk.szsharing.cn

Java: import java.util.List;
来源：http://dh.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rk.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://hn.huixiangedu.cn

C#:   using System.Text;
来源：http://at.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://mx.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://bf.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://qm.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://gh.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://lf.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rz.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ce.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://ja.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ps.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://sl.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://au.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://it.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lt.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bj.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iu.szsharing.cn

Go:   func add(a, b int) int
来源：http://yi.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jd.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uq.9csxet.cn

[C14] 泛型函数
来源：http://kj.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://la.panjiajie.cn

PHP:  // 无泛型
来源：http://ub.szsharing.cn

JS:   // 无泛型
来源：http://vs.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cv.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oq.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ad.hnjuh.cn

Ruby: # 无泛型
来源：http://uk.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yw.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://kz.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bw.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://pp.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yz.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ds.521024.cn

Java: // 无解构
来源：http://nz.haigaiapp.cn

Go:   // 无解构
来源：http://xl.gzmigu.cn

Ruby: a, b = pair
来源：http://sp.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://gz.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://yh.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vg.jianghongdianzi.cn

PHP:  // 无重载
来源：http://kl.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sp.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://lv.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rj.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://gw.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://uv.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xj.shxzskj.cn

================================================================================
来源：http://az.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://gf.jianghongdianzi.cn

================================================================================
来源：http://jl.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://fo.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sw.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gw.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sj.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xb.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ri.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://nm.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://qi.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rs.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://bo.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yx.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ul.nszjky.cn

JS:   arr.push(4);
来源：http://xk.shtwfgs.cn

TS:   arr.push(4);
来源：http://mk.521024.cn

Java: list.add(4);
来源：http://fp.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://on.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://gu.hnjuh.cn

C#:   list.Add(4);
来源：http://fs.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://un.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://zt.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ek.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vr.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://fz.panjiajie.cn

Java: list.add(0, 0);
来源：http://ry.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zp.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://si.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://ky.521024.cn

[D04] 删除元素
来源：http://oi.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ay.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hd.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wl.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://qz.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://je.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cf.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wg.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qx.szsharing.cn

[D05] 访问与修改元素
来源：http://ya.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jz.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qg.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kx.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ar.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://je.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ag.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xl.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bi.hnjuh.cn

[D06] 数组长度
来源：http://kz.panjiajie.cn

Py:   len(arr)
来源：http://ld.yuntaijiaju.cn

PHP:  count($arr);
来源：http://es.newstarts.cn

JS:   arr.length
来源：http://uf.chemitech.net.cn

TS:   arr.length
来源：http://uc.nicolike.cn

Java: list.size();
来源：http://ee.521024.cn

Go:   len(arr)
来源：http://iz.colortex.cn

Ruby: arr.length; arr.size
来源：http://oq.haigaiapp.cn

C#:   list.Count;
来源：http://ra.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://mo.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oo.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vi.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://ye.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://sg.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://gv.wgjwhj.cn

Go:   arr[1:4]
来源：http://vk.newstarts.cn

Ruby: arr[1, 3]
来源：http://hg.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ub.521024.cn

[D08] 合并两个数组
来源：http://oo.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://ob.asd995.cn

PHP:  array_merge($a, $b);
来源：http://ay.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vl.panjiajie.cn

TS:   [...a, ...b];
来源：http://gd.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aj.newstarts.cn

Go:   append(a, b...)
来源：http://rf.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://qr.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://qa.hahajie.cn

[D09] 排序（升序）
来源：http://og.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://dx.szsharing.cn

PHP:  sort($arr);
来源：http://uf.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tn.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ts.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yi.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qf.panjiajie.cn

Ruby: arr.sort
来源：http://dw.521024.cn

C#:   list.Sort();
来源：http://iy.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ur.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://as.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gt.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://al.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jo.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yu.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pc.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ju.shxzskj.cn

[D11] 反转数组
来源：http://kd.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://px.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://mt.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://la.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://no.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://gp.colortex.cn

Go:   slices.Reverse(arr)
来源：http://qr.hahajie.cn

Ruby: arr.reverse
来源：http://nr.9csxet.cn

C#:   list.Reverse();
来源：http://td.szsharing.cn

[D12] 查找元素下标
来源：http://nj.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://fh.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zg.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ca.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tx.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://up.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://op.nicolike.cn

Ruby: arr.index(x)
来源：http://it.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://do.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://wv.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tr.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://je.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://oq.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://xo.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://us.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ta.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pr.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bh.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://eg.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xx.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tu.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://tv.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://al.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://el.9csxet.cn

Go:   // 手写循环
来源：http://vv.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jf.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qr.lnxyls.cn

[D15] 去重
来源：http://cw.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ke.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://oc.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://hj.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://ie.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fl.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jb.yuexingan06.cn

Ruby: arr.uniq
来源：http://ej.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://ux.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ms.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dc.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fk.yuntaijiaju.cn


<!-- 参考信息 -->