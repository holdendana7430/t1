代发 wailian999

PHP:  $a && $b || !$c
来源：http://qd.wgjwhj.cn

JS:   a && b || !c
来源：http://fl.haigaiapp.cn

TS:   a && b || !c
来源：http://gb.nicolike.cn

Java: a && b || !c
来源：http://yr.jctech888.com.cn

Go:   a && b || !c
来源：http://mg.9csxet.cn

Ruby: a && b || !c
来源：http://xx.colortex.cn

C#:   a && b || !c
来源：http://tj.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://do.huixiangedu.cn

Py:   if not data: return
来源：http://mw.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://qq.shxzskj.cn

JS:   if (!data) return;
来源：http://lq.huanxung.cn

TS:   if (!data) return;
来源：http://ee.chemitech.net.cn

Java: if (data == null) return;
来源：http://du.9csxet.cn

Go:   if data == nil { return }
来源：http://zb.shxzskj.cn

Ruby: return if data.nil?
来源：http://dj.newstarts.cn

C#:   if (data == null) return;
来源：http://pg.newstarts.cn

================================================================================
来源：http://cq.521024.cn

C. 函数与作用域
来源：http://cp.shtwfgs.cn

================================================================================
来源：http://bg.gzmigu.cn

[C01] 定义函数
来源：http://st.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://cn.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://rn.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jv.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gm.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lj.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://lw.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bi.asd995.cn

[C02] 默认参数
来源：http://ec.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ye.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tf.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gk.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kz.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cr.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://si.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://bj.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://lb.szxytkj.cn

[C03] 可变参数
来源：http://yp.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://wq.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bo.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gu.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pp.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tp.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://af.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kd.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iw.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://vh.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gz.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mt.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bo.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zw.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://zs.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://la.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://eg.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://hh.gzmigu.cn

[C05] 返回多个值
来源：http://uc.gzmigu.cn

Py:   return a, b
来源：http://hf.shxzskj.cn

PHP:  return [$a, $b];
来源：http://pd.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mj.colortex.cn

TS:   return { a, b };
来源：http://vx.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ve.haigaiapp.cn

Go:   return a, b
来源：http://sl.haigaiapp.cn

Ruby: return a, b
来源：http://uv.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://hu.asd995.cn

[C06] 匿名函数 / lambda
来源：http://wl.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://ui.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ge.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://up.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://gv.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pc.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fp.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://fc.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pp.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://qx.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nc.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hc.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ts.hnjuh.cn

TS:   arr.map(String)
来源：http://ci.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gp.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hq.521024.cn

Ruby: arr.map(&:upcase)
来源：http://oo.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://th.jctech888.com.cn

[C08] 闭包
来源：http://um.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ph.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pg.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ju.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gr.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://za.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ur.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rm.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hb.hahajie.cn

[C09] 递归
来源：http://dd.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://av.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zj.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sl.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://im.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yv.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ru.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wf.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ip.colortex.cn

[C10] 变量作用域
来源：http://bf.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rs.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ku.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://af.panjiajie.cn

TS:   同 JS
来源：http://rf.lnxyls.cn

Java: 方法内为块级作用域
来源：http://so.hnjuh.cn

Go:   花括号块级作用域
来源：http://rn.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rz.shtwfgs.cn

C#:   块级作用域
来源：http://xx.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://yn.szxytkj.cn

Py:   from module import func
来源：http://wq.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rr.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://go.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cb.muxihuayi.cn

Java: import java.util.List;
来源：http://xn.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tc.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://hu.shxzskj.cn

C#:   using System.Text;
来源：http://my.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://af.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://zz.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://jc.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://re.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://mt.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nr.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://iu.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://xf.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fx.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://cv.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aj.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oj.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fu.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://io.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dx.9csxet.cn

Go:   func add(a, b int) int
来源：http://mg.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cu.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ys.521024.cn

[C14] 泛型函数
来源：http://hl.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sx.bjjhwx.cn

PHP:  // 无泛型
来源：http://ez.9csxet.cn

JS:   // 无泛型
来源：http://fa.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tk.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tk.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mk.jctech888.com.cn

Ruby: # 无泛型
来源：http://ty.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jm.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://mi.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ag.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://bp.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://az.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ix.521024.cn

Java: // 无解构
来源：http://jd.yuexingan06.cn

Go:   // 无解构
来源：http://yk.szxytkj.cn

Ruby: a, b = pair
来源：http://ga.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://jz.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://or.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wd.newstarts.cn

PHP:  // 无重载
来源：http://or.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fz.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://rr.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ft.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://vo.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://xh.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lm.shtwfgs.cn

================================================================================
来源：http://ix.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ob.jctech888.com.cn

================================================================================
来源：http://yf.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://pa.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eg.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://za.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ax.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kv.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cj.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://iv.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://cv.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bt.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://cf.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jv.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qo.gzmigu.cn

JS:   arr.push(4);
来源：http://zv.lnxyls.cn

TS:   arr.push(4);
来源：http://lu.yuntaijiaju.cn

Java: list.add(4);
来源：http://ki.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ni.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://pa.haigaiapp.cn

C#:   list.Add(4);
来源：http://gu.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://yq.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://sf.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fj.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pt.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://yw.hnjuh.cn

Java: list.add(0, 0);
来源：http://il.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rd.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nz.521024.cn

C#:   list.Insert(0, 0);
来源：http://io.panjiajie.cn

[D04] 删除元素
来源：http://yu.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ev.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xb.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yd.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://wf.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jw.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ji.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ty.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jg.huanxung.cn

[D05] 访问与修改元素
来源：http://eo.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pp.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sc.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qb.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://te.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://gp.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ww.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yc.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yv.gzmigu.cn

[D06] 数组长度
来源：http://iy.shtwfgs.cn

Py:   len(arr)
来源：http://lr.gzmigu.cn

PHP:  count($arr);
来源：http://kz.jctech888.com.cn

JS:   arr.length
来源：http://lb.szsharing.cn

TS:   arr.length
来源：http://vl.haigaiapp.cn

Java: list.size();
来源：http://yr.shxzskj.cn

Go:   len(arr)
来源：http://dj.521024.cn

Ruby: arr.length; arr.size
来源：http://fx.yuexingan06.cn

C#:   list.Count;
来源：http://aa.szsharing.cn

[D07] 切片 / 取子数组
来源：http://sb.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ya.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ou.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://cg.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://sx.shxzukj.cn

Java: list.subList(1, 4);
来源：http://oq.szsharing.cn

Go:   arr[1:4]
来源：http://vi.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://is.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://qd.lnxyls.cn

[D08] 合并两个数组
来源：http://ta.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://sl.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://jx.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zs.chemitech.net.cn

TS:   [...a, ...b];
来源：http://vl.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iv.gzmigu.cn

Go:   append(a, b...)
来源：http://zs.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://wb.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://yh.asd995.cn

[D09] 排序（升序）
来源：http://ij.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://uu.hnjuh.cn

PHP:  sort($arr);
来源：http://nm.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vp.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ss.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iw.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://or.huanxung.cn

Ruby: arr.sort
来源：http://ad.hnjuh.cn

C#:   list.Sort();
来源：http://fb.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eg.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ie.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ff.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vw.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rl.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ry.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lu.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rc.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bq.hnjuh.cn

[D11] 反转数组
来源：http://hc.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nv.nszjky.cn

PHP:  array_reverse($arr);
来源：http://si.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gd.nszjky.cn

TS:   [...arr].reverse();
来源：http://zr.hahajie.cn

Java: Collections.reverse(list);
来源：http://wm.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://yx.shxzskj.cn

Ruby: arr.reverse
来源：http://nk.bjjhwx.cn

C#:   list.Reverse();
来源：http://cx.colortex.cn

[D12] 查找元素下标
来源：http://ns.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://sf.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sy.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zz.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kk.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zj.asd995.cn

Go:   slices.Index(arr, x)
来源：http://yx.colortex.cn

Ruby: arr.index(x)
来源：http://ia.huanxung.cn

C#:   list.IndexOf(x);
来源：http://eq.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://ms.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pd.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qj.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://qb.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://sw.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qf.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vp.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xk.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sw.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://gr.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ec.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://yt.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://fp.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ml.huixiangedu.cn

Go:   // 手写循环
来源：http://yn.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ds.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fi.lnxyls.cn

[D15] 去重
来源：http://lj.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pd.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://es.huanxung.cn

JS:   [...new Set(arr)]
来源：http://vv.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://ah.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bt.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://op.szsharing.cn

Ruby: arr.uniq
来源：http://ig.bjjhwx.cn


<!-- 参考信息 -->