代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://du.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://st.panjiajie.cn

[B15] 布尔运算与取反
来源：http://df.shtwfgs.cn

Py:   a and b or not c
来源：http://rv.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://cv.asd995.cn

JS:   a && b || !c
来源：http://xx.szsharing.cn

TS:   a && b || !c
来源：http://uv.huanxung.cn

Java: a && b || !c
来源：http://ez.bookmarksfly.cn

Go:   a && b || !c
来源：http://bz.bjjhwx.cn

Ruby: a && b || !c
来源：http://ix.shxzukj.cn

C#:   a && b || !c
来源：http://tx.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ei.szxytkj.cn

Py:   if not data: return
来源：http://md.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://lm.yuexingan06.cn

JS:   if (!data) return;
来源：http://su.szxytkj.cn

TS:   if (!data) return;
来源：http://zc.colortex.cn

Java: if (data == null) return;
来源：http://sg.szsharing.cn

Go:   if data == nil { return }
来源：http://yc.shxzukj.cn

Ruby: return if data.nil?
来源：http://he.szxytkj.cn

C#:   if (data == null) return;
来源：http://yn.yuntaijiaju.cn

================================================================================
来源：http://oy.nszjky.cn

C. 函数与作用域
来源：http://il.colortex.cn

================================================================================
来源：http://tq.shxzskj.cn

[C01] 定义函数
来源：http://eb.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://dh.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yu.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://ql.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yv.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://do.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gn.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://hg.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ps.shxzskj.cn

[C02] 默认参数
来源：http://jp.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://bx.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pw.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://nt.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pa.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mk.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mm.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ep.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ko.huixinmuqiang.cn

[C03] 可变参数
来源：http://aa.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://ig.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://er.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tn.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://if.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hs.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ge.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ev.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fm.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ll.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ra.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qc.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jh.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ki.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://og.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://al.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://ue.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://gm.yuexingan06.cn

[C05] 返回多个值
来源：http://mb.huanxung.cn

Py:   return a, b
来源：http://gi.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://nd.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nl.shtwfgs.cn

TS:   return { a, b };
来源：http://yl.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qy.jctech888.com.cn

Go:   return a, b
来源：http://ys.panjiajie.cn

Ruby: return a, b
来源：http://vx.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://xi.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://qy.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://lh.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vr.nszjky.cn

JS:   const square = x => x * x;
来源：http://oj.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://pl.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gg.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sv.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://on.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lu.szsharing.cn

[C07] 把函数作为参数传入
来源：http://an.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fo.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gq.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yh.newstarts.cn

TS:   arr.map(String)
来源：http://xn.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sc.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yz.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://kl.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ux.asd995.cn

[C08] 闭包
来源：http://hv.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yj.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zg.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jv.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sr.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ql.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://at.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yg.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ib.colortex.cn

[C09] 递归
来源：http://fk.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zc.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jg.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vb.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sb.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lh.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tu.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ke.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xk.lnxyls.cn

[C10] 变量作用域
来源：http://fh.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pu.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://my.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sq.nszjky.cn

TS:   同 JS
来源：http://oj.hahajie.cn

Java: 方法内为块级作用域
来源：http://pa.nszjky.cn

Go:   花括号块级作用域
来源：http://bh.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ie.gzmigu.cn

C#:   块级作用域
来源：http://bq.nszjky.cn

[C11] 模块导入与导出
来源：http://ae.yuexingan06.cn

Py:   from module import func
来源：http://rk.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nq.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dt.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pg.shxzskj.cn

Java: import java.util.List;
来源：http://vt.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://us.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://yc.nicolike.cn

C#:   using System.Text;
来源：http://nd.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://cw.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://rw.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://yw.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://ip.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://rv.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kb.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://xz.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://ec.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yo.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://mu.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kg.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iz.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eg.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://po.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bs.9csxet.cn

Go:   func add(a, b int) int
来源：http://bf.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lw.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://op.huanxung.cn

[C14] 泛型函数
来源：http://ak.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vg.panjiajie.cn

PHP:  // 无泛型
来源：http://pm.huanxung.cn

JS:   // 无泛型
来源：http://it.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fx.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cv.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qu.gzmigu.cn

Ruby: # 无泛型
来源：http://cn.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cn.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ns.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ly.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://jw.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://te.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zs.panjiajie.cn

Java: // 无解构
来源：http://xc.lnxyls.cn

Go:   // 无解构
来源：http://vd.9csxet.cn

Ruby: a, b = pair
来源：http://uu.nicolike.cn

C#:   var (a, b) = pair;
来源：http://ut.521024.cn

[C16] 函数 / 方法重载
来源：http://ud.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zp.nszjky.cn

PHP:  // 无重载
来源：http://co.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ln.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://er.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bk.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://zu.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://bs.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cg.nszjky.cn

================================================================================
来源：http://mb.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://sl.shxzskj.cn

================================================================================
来源：http://rj.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://it.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tf.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nt.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hy.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xd.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ut.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zw.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://cv.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ma.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://hb.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://di.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iv.shxzskj.cn

JS:   arr.push(4);
来源：http://hy.wgjwhj.cn

TS:   arr.push(4);
来源：http://dl.521024.cn

Java: list.add(4);
来源：http://ez.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://pv.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://fu.yuexingan06.cn

C#:   list.Add(4);
来源：http://vc.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://lr.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://jt.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xm.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dy.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ts.shxzukj.cn

Java: list.add(0, 0);
来源：http://ta.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ux.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ib.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://sd.wgjwhj.cn

[D04] 删除元素
来源：http://ox.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fz.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://og.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dx.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://tz.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ac.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uy.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pg.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zv.lnxyls.cn

[D05] 访问与修改元素
来源：http://dl.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rz.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eq.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gi.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://gg.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://et.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ra.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bk.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vc.huixiangedu.cn

[D06] 数组长度
来源：http://vu.bookmarksfly.cn

Py:   len(arr)
来源：http://my.muxihuayi.cn

PHP:  count($arr);
来源：http://kz.shxzukj.cn

JS:   arr.length
来源：http://hr.asd995.cn

TS:   arr.length
来源：http://wt.hnjuh.cn

Java: list.size();
来源：http://hy.shxzskj.cn

Go:   len(arr)
来源：http://et.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://gk.hnjuh.cn

C#:   list.Count;
来源：http://cp.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://yr.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kr.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pb.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ff.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://rt.hnjuh.cn

Java: list.subList(1, 4);
来源：http://gz.szxytkj.cn

Go:   arr[1:4]
来源：http://ae.9csxet.cn

Ruby: arr[1, 3]
来源：http://ig.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ho.9csxet.cn

[D08] 合并两个数组
来源：http://oo.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ke.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://rp.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wo.nicolike.cn

TS:   [...a, ...b];
来源：http://bi.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nf.jctech888.com.cn

Go:   append(a, b...)
来源：http://iy.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://cg.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://aj.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://us.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://af.haigaiapp.cn

PHP:  sort($arr);
来源：http://vd.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nn.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://na.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wm.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jm.nicolike.cn

Ruby: arr.sort
来源：http://zx.jianghongdianzi.cn

C#:   list.Sort();
来源：http://tg.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wi.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://af.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ar.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mn.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qi.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://st.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nz.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dw.wgjwhj.cn

[D11] 反转数组
来源：http://pk.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gg.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://on.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uq.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ea.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://tc.asd995.cn

Go:   slices.Reverse(arr)
来源：http://aq.hnjuh.cn

Ruby: arr.reverse
来源：http://eh.szxytkj.cn

C#:   list.Reverse();
来源：http://jp.9csxet.cn

[D12] 查找元素下标
来源：http://cu.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ds.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wo.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fz.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mj.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pz.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://nf.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://vg.huanxung.cn

C#:   list.IndexOf(x);
来源：http://bd.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://va.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xg.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yo.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://ko.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://ao.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xc.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jy.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://er.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wc.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://fa.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jf.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wb.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://zs.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://ob.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://va.colortex.cn

Go:   // 手写循环
来源：http://tf.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mr.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rr.asd995.cn

[D15] 去重
来源：http://br.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ek.huanxung.cn

PHP:  array_unique($arr);
来源：http://kp.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://by.jianghongdianzi.cn


<!-- 参考信息 -->