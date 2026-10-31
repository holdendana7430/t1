代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://cc.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://bu.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qc.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fl.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ov.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ri.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://sx.huanxung.cn

Py:   a and b or not c
来源：http://zx.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://mc.nszjky.cn

JS:   a && b || !c
来源：http://fr.huixiangedu.cn

TS:   a && b || !c
来源：http://tp.huixiangedu.cn

Java: a && b || !c
来源：http://pg.lnxyls.cn

Go:   a && b || !c
来源：http://na.asd995.cn

Ruby: a && b || !c
来源：http://nr.shxzukj.cn

C#:   a && b || !c
来源：http://og.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ia.yuexingan06.cn

Py:   if not data: return
来源：http://lm.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://dm.muxihuayi.cn

JS:   if (!data) return;
来源：http://go.hnjuh.cn

TS:   if (!data) return;
来源：http://mp.szsharing.cn

Java: if (data == null) return;
来源：http://rs.nicolike.cn

Go:   if data == nil { return }
来源：http://zu.lnxyls.cn

Ruby: return if data.nil?
来源：http://bz.hnjuh.cn

C#:   if (data == null) return;
来源：http://kr.panjiajie.cn

================================================================================
来源：http://qs.nszjky.cn

C. 函数与作用域
来源：http://xl.huanxung.cn

================================================================================
来源：http://bh.szxytkj.cn

[C01] 定义函数
来源：http://js.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://gc.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://nq.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iv.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pf.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jn.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://mf.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pp.szsharing.cn

[C02] 默认参数
来源：http://ui.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ro.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xv.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://qk.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nj.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hk.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oj.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://bb.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://xq.9csxet.cn

[C03] 可变参数
来源：http://my.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://xn.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oq.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iw.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://da.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kg.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zq.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ke.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fo.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://cx.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yl.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lw.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yq.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ft.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ke.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://dh.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://af.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://jc.yuntaijiaju.cn

[C05] 返回多个值
来源：http://py.nszjky.cn

Py:   return a, b
来源：http://mr.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ob.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ty.nicolike.cn

TS:   return { a, b };
来源：http://wi.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rh.hnjuh.cn

Go:   return a, b
来源：http://zh.yuntaijiaju.cn

Ruby: return a, b
来源：http://fc.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://wt.asd995.cn

[C06] 匿名函数 / lambda
来源：http://sd.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://yf.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mq.lnxyls.cn

JS:   const square = x => x * x;
来源：http://aw.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://xx.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mb.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vr.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://gg.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kr.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://wa.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eo.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wt.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dz.nicolike.cn

TS:   arr.map(String)
来源：http://ua.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ik.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pw.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://wo.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://it.9csxet.cn

[C08] 闭包
来源：http://fv.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ur.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wm.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ol.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://au.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://am.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zj.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pn.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://et.nicolike.cn

[C09] 递归
来源：http://bg.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xs.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tr.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vc.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ku.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://st.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ox.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lo.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hu.gzmigu.cn

[C10] 变量作用域
来源：http://uw.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ku.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tk.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aj.wgjwhj.cn

TS:   同 JS
来源：http://ag.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://ca.newstarts.cn

Go:   花括号块级作用域
来源：http://gf.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jk.shxzukj.cn

C#:   块级作用域
来源：http://cw.hahajie.cn

[C11] 模块导入与导出
来源：http://eq.nszjky.cn

Py:   from module import func
来源：http://we.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lf.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xk.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ij.asd995.cn

Java: import java.util.List;
来源：http://op.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fc.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://xp.521024.cn

C#:   using System.Text;
来源：http://rs.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://ix.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://qv.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://by.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ha.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://jf.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ar.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://nh.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ug.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ie.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://nu.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xf.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xr.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://or.panjiajie.cn

Go:   func add(a, b int) int
来源：http://gz.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vm.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://go.wgjwhj.cn

[C14] 泛型函数
来源：http://mo.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pq.9csxet.cn

PHP:  // 无泛型
来源：http://ub.szsharing.cn

JS:   // 无泛型
来源：http://uu.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iw.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ik.lnxyls.cn

Ruby: # 无泛型
来源：http://gy.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://je.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://xg.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pi.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://oa.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rx.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://db.jianghongdianzi.cn

Java: // 无解构
来源：http://fc.panjiajie.cn

Go:   // 无解构
来源：http://kz.newstarts.cn

Ruby: a, b = pair
来源：http://xd.9csxet.cn

C#:   var (a, b) = pair;
来源：http://kk.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://zu.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xc.nszjky.cn

PHP:  // 无重载
来源：http://br.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rn.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://rd.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ri.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://fd.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://is.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qp.shxzukj.cn

================================================================================
来源：http://ig.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://to.huixiangedu.cn

================================================================================
来源：http://ei.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://ok.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wp.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yc.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hc.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ed.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rv.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://fo.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://vi.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sh.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://cl.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tq.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mg.hnjuh.cn

JS:   arr.push(4);
来源：http://sw.haigaiapp.cn

TS:   arr.push(4);
来源：http://lw.hahajie.cn

Java: list.add(4);
来源：http://fs.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://aa.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://jd.shtwfgs.cn

C#:   list.Add(4);
来源：http://er.nszjky.cn

[D03] 在指定位置插入元素
来源：http://oc.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://si.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rm.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zc.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ru.chemitech.net.cn

Java: list.add(0, 0);
来源：http://um.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bs.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://to.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://fr.gzmigu.cn

[D04] 删除元素
来源：http://nn.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bi.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zc.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xf.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://qz.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zp.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eb.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xp.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vz.szxytkj.cn

[D05] 访问与修改元素
来源：http://rh.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ik.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qf.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lh.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://hm.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://fq.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ca.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kc.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iy.nszjky.cn

[D06] 数组长度
来源：http://hl.nicolike.cn

Py:   len(arr)
来源：http://fx.nszjky.cn

PHP:  count($arr);
来源：http://wk.szsharing.cn

JS:   arr.length
来源：http://pm.bookmarksfly.cn

TS:   arr.length
来源：http://po.yuexingan06.cn

Java: list.size();
来源：http://ns.nszjky.cn

Go:   len(arr)
来源：http://tv.9csxet.cn

Ruby: arr.length; arr.size
来源：http://os.panjiajie.cn

C#:   list.Count;
来源：http://ks.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ae.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ax.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qe.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://vy.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://nd.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://co.shtwfgs.cn

Go:   arr[1:4]
来源：http://mx.shxzukj.cn

Ruby: arr[1, 3]
来源：http://kq.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://wi.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://na.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://fa.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://or.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ur.colortex.cn

TS:   [...a, ...b];
来源：http://gt.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rz.asd995.cn

Go:   append(a, b...)
来源：http://ea.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://ch.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://xf.nicolike.cn

[D09] 排序（升序）
来源：http://zu.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://gu.yuexingan06.cn

PHP:  sort($arr);
来源：http://ig.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://da.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uh.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zn.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nb.bjjhwx.cn

Ruby: arr.sort
来源：http://wo.jctech888.com.cn

C#:   list.Sort();
来源：http://rx.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uf.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://up.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ls.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jl.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nf.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qp.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lo.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://od.wgjwhj.cn

[D11] 反转数组
来源：http://xw.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yt.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://li.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rf.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://mz.asd995.cn

Java: Collections.reverse(list);
来源：http://mm.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://hm.shtwfgs.cn

Ruby: arr.reverse
来源：http://xw.hnjuh.cn

C#:   list.Reverse();
来源：http://gz.haigaiapp.cn

[D12] 查找元素下标
来源：http://pj.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://yh.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ci.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gx.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ic.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wv.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://cu.521024.cn

Ruby: arr.index(x)
来源：http://tw.521024.cn

C#:   list.IndexOf(x);
来源：http://tx.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://wb.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yq.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fu.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://rs.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://mr.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bw.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rj.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ia.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vj.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://vn.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yr.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vm.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ka.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://jn.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hm.szxytkj.cn

Go:   // 手写循环
来源：http://bj.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ci.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nh.shxzskj.cn


<!-- 参考信息 -->