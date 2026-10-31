代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://zb.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://li.nicolike.cn

[B15] 布尔运算与取反
来源：http://ca.9csxet.cn

Py:   a and b or not c
来源：http://rq.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://jb.haigaiapp.cn

JS:   a && b || !c
来源：http://ey.muxihuayi.cn

TS:   a && b || !c
来源：http://zx.szxytkj.cn

Java: a && b || !c
来源：http://br.muxihuayi.cn

Go:   a && b || !c
来源：http://ik.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ie.wgjwhj.cn

C#:   a && b || !c
来源：http://ft.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rh.lnxyls.cn

Py:   if not data: return
来源：http://zk.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://qn.nszjky.cn

JS:   if (!data) return;
来源：http://bw.hnjuh.cn

TS:   if (!data) return;
来源：http://zz.colortex.cn

Java: if (data == null) return;
来源：http://ca.szxytkj.cn

Go:   if data == nil { return }
来源：http://ld.szxytkj.cn

Ruby: return if data.nil?
来源：http://bu.huixiangedu.cn

C#:   if (data == null) return;
来源：http://er.gzmigu.cn

================================================================================
来源：http://ei.muxihuayi.cn

C. 函数与作用域
来源：http://al.shxzukj.cn

================================================================================
来源：http://je.szxytkj.cn

[C01] 定义函数
来源：http://cj.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ti.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ic.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://lh.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ai.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pw.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://cy.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hi.hahajie.cn

[C02] 默认参数
来源：http://nr.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://wx.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kg.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://pi.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vt.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dw.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lw.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://nt.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://bj.hnjuh.cn

[C03] 可变参数
来源：http://cp.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://eb.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ad.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cu.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vc.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oe.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ft.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uj.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oy.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://nv.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://og.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fv.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vo.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cy.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://og.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ud.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://lf.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://uv.huixiangedu.cn

[C05] 返回多个值
来源：http://ch.shxzukj.cn

Py:   return a, b
来源：http://we.shxzukj.cn

PHP:  return [$a, $b];
来源：http://dz.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ys.gzmigu.cn

TS:   return { a, b };
来源：http://qi.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nl.9csxet.cn

Go:   return a, b
来源：http://es.wgjwhj.cn

Ruby: return a, b
来源：http://dn.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://uy.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://py.huanxung.cn

Py:   square = lambda x: x * x
来源：http://uc.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nn.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://fm.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ai.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gx.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wf.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://ek.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rn.asd995.cn

[C07] 把函数作为参数传入
来源：http://ij.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ps.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ra.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bf.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://ga.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cc.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kd.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://qt.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kc.huixinmuqiang.cn

[C08] 闭包
来源：http://mp.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cc.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oi.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pb.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eh.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eu.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jd.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ed.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qk.asd995.cn

[C09] 递归
来源：http://es.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bo.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wb.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jp.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ja.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pt.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dy.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uy.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lb.colortex.cn

[C10] 变量作用域
来源：http://it.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ff.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bh.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qh.hahajie.cn

TS:   同 JS
来源：http://gg.newstarts.cn

Java: 方法内为块级作用域
来源：http://nc.bjjhwx.cn

Go:   花括号块级作用域
来源：http://cw.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tp.muxihuayi.cn

C#:   块级作用域
来源：http://go.521024.cn

[C11] 模块导入与导出
来源：http://ex.9csxet.cn

Py:   from module import func
来源：http://po.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vp.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gu.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gh.hnjuh.cn

Java: import java.util.List;
来源：http://xz.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yl.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ge.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ky.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://iw.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://tz.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://gn.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://cm.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://nx.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jg.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://fg.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://rv.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rc.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://vf.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dt.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ch.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gl.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gr.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vf.9csxet.cn

Go:   func add(a, b int) int
来源：http://qx.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nu.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bd.bookmarksfly.cn

[C14] 泛型函数
来源：http://ay.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cr.yuexingan06.cn

PHP:  // 无泛型
来源：http://kk.huixinmuqiang.cn

JS:   // 无泛型
来源：http://zt.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gj.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qn.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://za.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://hi.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qi.hahajie.cn

[C15] 解构 / 展开参数
来源：http://bu.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oi.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://uj.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bs.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yb.szxytkj.cn

Java: // 无解构
来源：http://ea.bookmarksfly.cn

Go:   // 无解构
来源：http://zv.hnjuh.cn

Ruby: a, b = pair
来源：http://rz.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://gm.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ir.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ey.nszjky.cn

PHP:  // 无重载
来源：http://mr.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ll.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://aa.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rz.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://kq.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://yk.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uk.shtwfgs.cn

================================================================================
来源：http://vp.asd995.cn

D. 数组 / 列表 / 集合
来源：http://xz.szxytkj.cn

================================================================================
来源：http://nn.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://or.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mw.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ih.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aa.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vw.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://up.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://lv.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://hr.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qv.hahajie.cn

[D02] 追加元素到末尾
来源：http://to.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://if.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dd.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://qb.521024.cn

TS:   arr.push(4);
来源：http://at.panjiajie.cn

Java: list.add(4);
来源：http://rs.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://tv.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://qo.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://sx.szsharing.cn

[D03] 在指定位置插入元素
来源：http://ih.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://sr.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gr.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ay.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://km.szsharing.cn

Java: list.add(0, 0);
来源：http://te.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hv.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ev.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://sq.huixinmuqiang.cn

[D04] 删除元素
来源：http://la.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eg.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nm.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://km.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://cv.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pf.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fl.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zl.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ii.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://pw.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vz.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sd.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iu.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ml.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://yt.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://sr.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lm.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ig.bjjhwx.cn

[D06] 数组长度
来源：http://by.9csxet.cn

Py:   len(arr)
来源：http://ed.shxzskj.cn

PHP:  count($arr);
来源：http://md.wgjwhj.cn

JS:   arr.length
来源：http://wa.nszjky.cn

TS:   arr.length
来源：http://zs.haigaiapp.cn

Java: list.size();
来源：http://pk.nicolike.cn

Go:   len(arr)
来源：http://kf.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://ut.yuntaijiaju.cn

C#:   list.Count;
来源：http://io.asd995.cn

[D07] 切片 / 取子数组
来源：http://cb.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zv.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gz.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://zw.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://fw.szsharing.cn

Java: list.subList(1, 4);
来源：http://di.szxytkj.cn

Go:   arr[1:4]
来源：http://dy.shxzskj.cn

Ruby: arr[1, 3]
来源：http://vb.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://pf.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://fm.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://sa.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://er.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ge.huixiangedu.cn

TS:   [...a, ...b];
来源：http://tj.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ok.hahajie.cn

Go:   append(a, b...)
来源：http://be.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://jr.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://mb.nicolike.cn

[D09] 排序（升序）
来源：http://rt.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fq.nicolike.cn

PHP:  sort($arr);
来源：http://xm.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bn.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yg.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ra.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://to.shtwfgs.cn

Ruby: arr.sort
来源：http://ir.szsharing.cn

C#:   list.Sort();
来源：http://ur.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dv.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ge.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fh.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rn.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://he.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nj.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://me.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kg.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xo.bjjhwx.cn

[D11] 反转数组
来源：http://nr.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hi.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://do.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ui.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://yt.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://tq.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://wv.huixiangedu.cn

Ruby: arr.reverse
来源：http://va.bjjhwx.cn

C#:   list.Reverse();
来源：http://fp.hnjuh.cn

[D12] 查找元素下标
来源：http://gt.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://rs.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mn.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zz.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xz.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xs.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://ra.jctech888.com.cn

Ruby: arr.index(x)
来源：http://vl.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://ad.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://wj.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ez.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://em.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://od.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ef.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wq.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yf.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pb.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://df.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://pa.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qm.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sb.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://hx.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://wd.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xj.521024.cn

Go:   // 手写循环
来源：http://si.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://us.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ya.gzmigu.cn

[D15] 去重
来源：http://lp.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cj.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://lv.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://uq.bookmarksfly.cn


<!-- 参考信息 -->