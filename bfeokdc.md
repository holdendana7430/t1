代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://sz.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lr.9csxet.cn

[B15] 布尔运算与取反
来源：http://oj.shxzukj.cn

Py:   a and b or not c
来源：http://zy.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://uw.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ze.shxzskj.cn

TS:   a && b || !c
来源：http://lu.shxzskj.cn

Java: a && b || !c
来源：http://pu.hahajie.cn

Go:   a && b || !c
来源：http://tl.szxytkj.cn

Ruby: a && b || !c
来源：http://mx.bjjhwx.cn

C#:   a && b || !c
来源：http://po.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wd.shxzskj.cn

Py:   if not data: return
来源：http://pj.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://bb.hnjuh.cn

JS:   if (!data) return;
来源：http://ht.wgjwhj.cn

TS:   if (!data) return;
来源：http://ik.huanxung.cn

Java: if (data == null) return;
来源：http://mc.panjiajie.cn

Go:   if data == nil { return }
来源：http://jr.yuexingan06.cn

Ruby: return if data.nil?
来源：http://aj.bjjhwx.cn

C#:   if (data == null) return;
来源：http://hw.asd995.cn

================================================================================
来源：http://ww.chemitech.net.cn

C. 函数与作用域
来源：http://er.shxzukj.cn

================================================================================
来源：http://sf.shtwfgs.cn

[C01] 定义函数
来源：http://qg.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://gm.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hv.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://po.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bc.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wd.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ue.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://pi.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cf.9csxet.cn

[C02] 默认参数
来源：http://gu.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://ql.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ny.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ca.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vu.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gu.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bb.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ce.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://jm.wgjwhj.cn

[C03] 可变参数
来源：http://od.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://ci.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://le.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mc.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jb.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xc.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ja.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://vv.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gg.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ts.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xv.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vn.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://bp.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://ct.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://em.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://mz.521024.cn

[C05] 返回多个值
来源：http://lw.jctech888.com.cn

Py:   return a, b
来源：http://jh.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://lj.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nd.9csxet.cn

TS:   return { a, b };
来源：http://al.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ul.newstarts.cn

Go:   return a, b
来源：http://vf.hahajie.cn

Ruby: return a, b
来源：http://nn.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://rj.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://ql.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://md.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ee.hahajie.cn

JS:   const square = x => x * x;
来源：http://ji.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ej.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iv.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tc.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://tf.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://or.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://fp.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sa.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ne.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ue.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://ku.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bv.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vg.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://ch.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sq.newstarts.cn

[C08] 闭包
来源：http://gt.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jy.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fw.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mc.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sz.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sm.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://le.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ny.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://io.szxytkj.cn

[C09] 递归
来源：http://ub.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kx.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://as.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://it.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ya.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://au.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tm.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oe.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cw.nicolike.cn

[C10] 变量作用域
来源：http://rz.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cc.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://um.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wz.muxihuayi.cn

TS:   同 JS
来源：http://cd.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://fb.asd995.cn

Go:   花括号块级作用域
来源：http://zs.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cu.nicolike.cn

C#:   块级作用域
来源：http://mb.shxzukj.cn

[C11] 模块导入与导出
来源：http://ve.hnjuh.cn

Py:   from module import func
来源：http://jy.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cd.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lj.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ja.bjjhwx.cn

Java: import java.util.List;
来源：http://wr.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ar.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://qw.wgjwhj.cn

C#:   using System.Text;
来源：http://mj.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://on.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://er.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://yi.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://uw.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://xl.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rf.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xi.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://hw.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cv.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://gv.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mv.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mj.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bm.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sg.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bw.lnxyls.cn

Go:   func add(a, b int) int
来源：http://rj.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wh.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bs.chemitech.net.cn

[C14] 泛型函数
来源：http://pn.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://se.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://qn.521024.cn

JS:   // 无泛型
来源：http://mt.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iy.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ke.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eo.newstarts.cn

Ruby: # 无泛型
来源：http://kx.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pa.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ug.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hc.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://tq.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xv.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gb.huanxung.cn

Java: // 无解构
来源：http://to.bookmarksfly.cn

Go:   // 无解构
来源：http://sy.jctech888.com.cn

Ruby: a, b = pair
来源：http://xm.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://ws.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://wi.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yw.huixiangedu.cn

PHP:  // 无重载
来源：http://gz.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ue.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gq.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wp.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://is.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://dq.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dq.lnxyls.cn

================================================================================
来源：http://av.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://uc.shxzskj.cn

================================================================================
来源：http://az.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://oc.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qq.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bc.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bp.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gk.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bi.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rq.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://te.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://su.9csxet.cn

[D02] 追加元素到末尾
来源：http://fp.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qe.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qv.521024.cn

JS:   arr.push(4);
来源：http://ub.yuexingan06.cn

TS:   arr.push(4);
来源：http://oo.muxihuayi.cn

Java: list.add(4);
来源：http://yv.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://co.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jn.shxzskj.cn

C#:   list.Add(4);
来源：http://wd.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://xl.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://tz.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tn.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ol.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://qd.jctech888.com.cn

Java: list.add(0, 0);
来源：http://po.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zc.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hb.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://qy.chemitech.net.cn

[D04] 删除元素
来源：http://cg.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vz.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cl.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mr.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://fv.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rv.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bo.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yu.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rh.asd995.cn

[D05] 访问与修改元素
来源：http://tm.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cc.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://br.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://de.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://vv.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://lq.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://li.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zk.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kl.szxytkj.cn

[D06] 数组长度
来源：http://iu.colortex.cn

Py:   len(arr)
来源：http://fk.huixiangedu.cn

PHP:  count($arr);
来源：http://ag.wgjwhj.cn

JS:   arr.length
来源：http://os.haigaiapp.cn

TS:   arr.length
来源：http://xj.colortex.cn

Java: list.size();
来源：http://jn.shxzukj.cn

Go:   len(arr)
来源：http://fw.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://jd.newstarts.cn

C#:   list.Count;
来源：http://qt.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ka.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ua.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://od.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://eb.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://df.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://cs.wgjwhj.cn

Go:   arr[1:4]
来源：http://wg.hnjuh.cn

Ruby: arr[1, 3]
来源：http://uq.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://hj.shtwfgs.cn

[D08] 合并两个数组
来源：http://bh.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://hw.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://mn.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jd.shxzukj.cn

TS:   [...a, ...b];
来源：http://bc.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nn.shtwfgs.cn

Go:   append(a, b...)
来源：http://uc.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://mx.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://bl.521024.cn

[D09] 排序（升序）
来源：http://gu.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://kk.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://hd.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qq.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gn.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zd.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ii.shxzskj.cn

Ruby: arr.sort
来源：http://vv.shxzukj.cn

C#:   list.Sort();
来源：http://cu.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pi.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mx.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pa.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ke.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yw.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qv.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://je.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ag.muxihuayi.cn

[D11] 反转数组
来源：http://fo.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qj.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://hz.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fs.nszjky.cn

TS:   [...arr].reverse();
来源：http://yp.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ww.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://pz.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://kk.bookmarksfly.cn

C#:   list.Reverse();
来源：http://pg.huixiangedu.cn

[D12] 查找元素下标
来源：http://xx.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://wn.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vf.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://av.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fd.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jc.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://sa.nszjky.cn

Ruby: arr.index(x)
来源：http://jq.hahajie.cn

C#:   list.IndexOf(x);
来源：http://xz.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://pv.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kh.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bm.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ni.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://iz.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rs.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ow.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tj.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vh.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://nj.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rj.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ew.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://du.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://tz.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sb.shxzukj.cn

Go:   // 手写循环
来源：http://yk.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lz.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fy.newstarts.cn

[D15] 去重
来源：http://sa.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qr.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://oy.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://sj.shxzskj.cn


<!-- 参考信息 -->