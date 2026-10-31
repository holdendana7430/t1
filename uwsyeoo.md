代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ri.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zh.521024.cn

[B15] 布尔运算与取反
来源：http://kt.yuexingan06.cn

Py:   a and b or not c
来源：http://mb.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://eh.jianghongdianzi.cn

JS:   a && b || !c
来源：http://mv.lnxyls.cn

TS:   a && b || !c
来源：http://rf.521024.cn

Java: a && b || !c
来源：http://py.szxytkj.cn

Go:   a && b || !c
来源：http://oo.chemitech.net.cn

Ruby: a && b || !c
来源：http://kx.chemitech.net.cn

C#:   a && b || !c
来源：http://bp.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gt.huanxung.cn

Py:   if not data: return
来源：http://if.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://za.lnxyls.cn

JS:   if (!data) return;
来源：http://nc.shxzukj.cn

TS:   if (!data) return;
来源：http://np.nicolike.cn

Java: if (data == null) return;
来源：http://bz.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://eh.newstarts.cn

Ruby: return if data.nil?
来源：http://iz.newstarts.cn

C#:   if (data == null) return;
来源：http://si.shxzukj.cn

================================================================================
来源：http://vm.shxzskj.cn

C. 函数与作用域
来源：http://bl.muxihuayi.cn

================================================================================
来源：http://hy.9csxet.cn

[C01] 定义函数
来源：http://yl.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://si.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mp.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://mh.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ae.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sl.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dy.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://ad.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ne.yuntaijiaju.cn

[C02] 默认参数
来源：http://wf.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://dy.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ks.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://lx.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mf.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fa.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eq.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://pf.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://il.yuntaijiaju.cn

[C03] 可变参数
来源：http://ai.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://bq.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uf.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://in.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pj.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rx.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qw.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jg.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mx.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://sr.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bw.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://su.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://by.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://da.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://vp.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://rw.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://gu.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://qb.muxihuayi.cn

[C05] 返回多个值
来源：http://aa.newstarts.cn

Py:   return a, b
来源：http://dm.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://wc.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fh.szsharing.cn

TS:   return { a, b };
来源：http://gy.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://io.hnjuh.cn

Go:   return a, b
来源：http://gj.huanxung.cn

Ruby: return a, b
来源：http://ro.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://uv.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://nn.asd995.cn

Py:   square = lambda x: x * x
来源：http://dd.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vj.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://ru.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://bm.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vf.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qt.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://la.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nh.newstarts.cn

[C07] 把函数作为参数传入
来源：http://bj.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jw.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ou.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ck.hahajie.cn

TS:   arr.map(String)
来源：http://ko.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://et.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://te.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://rf.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ff.asd995.cn

[C08] 闭包
来源：http://wb.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iu.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pn.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zm.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ws.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ow.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hl.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ny.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lz.szsharing.cn

[C09] 递归
来源：http://rq.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xn.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lv.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gt.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gy.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ak.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sk.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fh.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lo.yuntaijiaju.cn

[C10] 变量作用域
来源：http://qj.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bm.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vc.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cg.jianghongdianzi.cn

TS:   同 JS
来源：http://ip.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ol.gzmigu.cn

Go:   花括号块级作用域
来源：http://gi.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ta.chemitech.net.cn

C#:   块级作用域
来源：http://ey.9csxet.cn

[C11] 模块导入与导出
来源：http://zx.colortex.cn

Py:   from module import func
来源：http://if.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jj.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qw.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://em.gzmigu.cn

Java: import java.util.List;
来源：http://he.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dk.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://hw.gzmigu.cn

C#:   using System.Text;
来源：http://qz.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://cs.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://qc.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://et.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://jd.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://yq.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gz.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pf.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://pb.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zh.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://zv.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mq.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gd.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://do.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fc.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://zp.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ng.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zd.chemitech.net.cn

[C14] 泛型函数
来源：http://pj.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sd.asd995.cn

PHP:  // 无泛型
来源：http://rh.jctech888.com.cn

JS:   // 无泛型
来源：http://rd.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cw.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qb.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ss.shxzskj.cn

Ruby: # 无泛型
来源：http://ue.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://md.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://gs.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ql.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://tp.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ec.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://az.jianghongdianzi.cn

Java: // 无解构
来源：http://xz.lnxyls.cn

Go:   // 无解构
来源：http://py.shtwfgs.cn

Ruby: a, b = pair
来源：http://mz.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://pu.9csxet.cn

[C16] 函数 / 方法重载
来源：http://dp.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mn.shtwfgs.cn

PHP:  // 无重载
来源：http://er.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://an.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://jh.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ln.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://rh.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://ae.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pt.colortex.cn

================================================================================
来源：http://gf.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://mi.yuexingan06.cn

================================================================================
来源：http://bj.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://jg.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wh.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zo.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://at.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qh.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kn.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://iu.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://bk.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fe.521024.cn

[D02] 追加元素到末尾
来源：http://ef.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ca.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uk.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ab.bookmarksfly.cn

TS:   arr.push(4);
来源：http://ta.9csxet.cn

Java: list.add(4);
来源：http://dc.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://ui.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://bp.panjiajie.cn

C#:   list.Add(4);
来源：http://hp.nszjky.cn

[D03] 在指定位置插入元素
来源：http://tc.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://ri.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hg.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qp.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://ei.chemitech.net.cn

Java: list.add(0, 0);
来源：http://xj.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mi.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uv.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://ws.bjjhwx.cn

[D04] 删除元素
来源：http://mj.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pb.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qn.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uw.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://tu.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wd.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bt.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xy.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gt.huixiangedu.cn

[D05] 访问与修改元素
来源：http://ad.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://li.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lo.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gy.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://de.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://yw.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://my.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gp.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xk.521024.cn

[D06] 数组长度
来源：http://xb.jctech888.com.cn

Py:   len(arr)
来源：http://fk.yuntaijiaju.cn

PHP:  count($arr);
来源：http://lt.bjjhwx.cn

JS:   arr.length
来源：http://fo.bookmarksfly.cn

TS:   arr.length
来源：http://ue.521024.cn

Java: list.size();
来源：http://an.shxzukj.cn

Go:   len(arr)
来源：http://gk.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ym.huixinmuqiang.cn

C#:   list.Count;
来源：http://jc.asd995.cn

[D07] 切片 / 取子数组
来源：http://nk.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://al.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://at.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://ag.colortex.cn

TS:   arr.slice(1, 4);
来源：http://cf.nszjky.cn

Java: list.subList(1, 4);
来源：http://ow.haigaiapp.cn

Go:   arr[1:4]
来源：http://jl.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://vb.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://sf.huanxung.cn

[D08] 合并两个数组
来源：http://sa.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://xi.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://ay.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ms.yuexingan06.cn

TS:   [...a, ...b];
来源：http://da.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://em.asd995.cn

Go:   append(a, b...)
来源：http://af.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://is.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://fd.wgjwhj.cn

[D09] 排序（升序）
来源：http://cr.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kz.nszjky.cn

PHP:  sort($arr);
来源：http://jn.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ml.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ah.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pr.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ja.chemitech.net.cn

Ruby: arr.sort
来源：http://tl.asd995.cn

C#:   list.Sort();
来源：http://rz.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kt.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ll.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wg.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ge.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uv.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ef.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tt.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qs.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qt.521024.cn

[D11] 反转数组
来源：http://gm.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://su.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://sq.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lc.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://ui.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://be.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://af.shxzskj.cn

Ruby: arr.reverse
来源：http://az.huixiangedu.cn

C#:   list.Reverse();
来源：http://gu.gzmigu.cn

[D12] 查找元素下标
来源：http://ig.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ze.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fg.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bb.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iz.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ne.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://dt.chemitech.net.cn

Ruby: arr.index(x)
来源：http://zx.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://np.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://xa.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vn.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ag.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://xt.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ic.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://km.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tf.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://di.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ki.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://gl.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gy.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zr.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://wo.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://pi.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wh.colortex.cn

Go:   // 手写循环
来源：http://tg.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://do.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hw.shxzskj.cn

[D15] 去重
来源：http://yf.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vj.panjiajie.cn

PHP:  array_unique($arr);
来源：http://kz.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://vk.bookmarksfly.cn


<!-- 参考信息 -->