代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://qg.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://un.lnxyls.cn

[B15] 布尔运算与取反
来源：http://lz.9csxet.cn

Py:   a and b or not c
来源：http://aa.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://mh.hahajie.cn

JS:   a && b || !c
来源：http://ro.hnjuh.cn

TS:   a && b || !c
来源：http://xh.shtwfgs.cn

Java: a && b || !c
来源：http://ip.521024.cn

Go:   a && b || !c
来源：http://rj.lnxyls.cn

Ruby: a && b || !c
来源：http://dc.panjiajie.cn

C#:   a && b || !c
来源：http://st.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://do.9csxet.cn

Py:   if not data: return
来源：http://ah.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ob.newstarts.cn

JS:   if (!data) return;
来源：http://go.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://yz.muxihuayi.cn

Java: if (data == null) return;
来源：http://po.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ue.shtwfgs.cn

Ruby: return if data.nil?
来源：http://lx.muxihuayi.cn

C#:   if (data == null) return;
来源：http://eg.nszjky.cn

================================================================================
来源：http://bz.bjjhwx.cn

C. 函数与作用域
来源：http://mw.shxzskj.cn

================================================================================
来源：http://vj.szxytkj.cn

[C01] 定义函数
来源：http://hp.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://fi.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://pm.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uc.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ge.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dv.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://gt.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yg.newstarts.cn

[C02] 默认参数
来源：http://hr.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://wb.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jv.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://if.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ui.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fn.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mz.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://pu.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://dh.newstarts.cn

[C03] 可变参数
来源：http://zl.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://gi.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gm.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qv.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zz.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jm.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lh.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ox.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ey.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yv.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fh.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gk.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nl.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://kc.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ll.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://il.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://ja.yuntaijiaju.cn

[C05] 返回多个值
来源：http://se.shtwfgs.cn

Py:   return a, b
来源：http://bp.nicolike.cn

PHP:  return [$a, $b];
来源：http://zq.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ao.yuexingan06.cn

TS:   return { a, b };
来源：http://zm.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ay.newstarts.cn

Go:   return a, b
来源：http://kh.huanxung.cn

Ruby: return a, b
来源：http://jz.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://hk.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://kr.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://jk.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jy.szsharing.cn

JS:   const square = x => x * x;
来源：http://ew.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ry.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jz.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xm.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://qj.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qc.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://wo.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qb.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dn.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xk.asd995.cn

TS:   arr.map(String)
来源：http://lm.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yb.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kw.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://sn.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tc.asd995.cn

[C08] 闭包
来源：http://hc.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://er.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wf.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fa.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ib.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zc.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fg.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ui.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dv.yuexingan06.cn

[C09] 递归
来源：http://hh.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qe.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sm.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zk.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vu.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ow.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xw.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zn.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ad.szsharing.cn

[C10] 变量作用域
来源：http://cl.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qj.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hp.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oq.lnxyls.cn

TS:   同 JS
来源：http://hc.huanxung.cn

Java: 方法内为块级作用域
来源：http://yx.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ay.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cv.panjiajie.cn

C#:   块级作用域
来源：http://xv.nszjky.cn

[C11] 模块导入与导出
来源：http://gp.nicolike.cn

Py:   from module import func
来源：http://op.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cb.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mp.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ka.szxytkj.cn

Java: import java.util.List;
来源：http://xd.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://at.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://go.yuexingan06.cn

C#:   using System.Text;
来源：http://oo.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://ha.colortex.cn

Py:   (lambda: print("run"))()
来源：http://nj.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://xa.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ue.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://sz.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ug.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://lt.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://li.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ff.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://dz.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fo.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ie.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oi.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yz.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://it.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://av.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dj.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qh.nicolike.cn

[C14] 泛型函数
来源：http://vm.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wk.shxzukj.cn

PHP:  // 无泛型
来源：http://dj.szsharing.cn

JS:   // 无泛型
来源：http://rd.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jg.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://en.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dk.szsharing.cn

Ruby: # 无泛型
来源：http://ls.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://en.nicolike.cn

[C15] 解构 / 展开参数
来源：http://kg.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qe.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://of.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bt.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nr.yuntaijiaju.cn

Java: // 无解构
来源：http://qh.521024.cn

Go:   // 无解构
来源：http://mb.szsharing.cn

Ruby: a, b = pair
来源：http://sg.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://kl.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://vm.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gz.huixiangedu.cn

PHP:  // 无重载
来源：http://su.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://it.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://fk.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://la.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://ja.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://oh.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yq.panjiajie.cn

================================================================================
来源：http://ng.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://yh.yuntaijiaju.cn

================================================================================
来源：http://gr.nszjky.cn

[D01] 创建数组 / 列表
来源：http://qp.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://td.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://es.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ji.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://js.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zq.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://gb.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://tt.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qy.huanxung.cn

[D02] 追加元素到末尾
来源：http://jv.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tv.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kg.huanxung.cn

JS:   arr.push(4);
来源：http://ia.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://st.shtwfgs.cn

Java: list.add(4);
来源：http://fn.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://wk.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://xf.szxytkj.cn

C#:   list.Add(4);
来源：http://xa.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://qb.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://ob.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ah.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ro.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://br.huanxung.cn

Java: list.add(0, 0);
来源：http://fc.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://is.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wg.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ho.nszjky.cn

[D04] 删除元素
来源：http://si.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ws.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sm.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ce.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://xr.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lz.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nf.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ir.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://id.hahajie.cn

[D05] 访问与修改元素
来源：http://dv.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vf.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jw.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ir.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://rt.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://xe.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://oi.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://de.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xw.shtwfgs.cn

[D06] 数组长度
来源：http://yz.szxytkj.cn

Py:   len(arr)
来源：http://so.chemitech.net.cn

PHP:  count($arr);
来源：http://kg.haigaiapp.cn

JS:   arr.length
来源：http://ow.shtwfgs.cn

TS:   arr.length
来源：http://jt.shxzskj.cn

Java: list.size();
来源：http://kz.bookmarksfly.cn

Go:   len(arr)
来源：http://pr.asd995.cn

Ruby: arr.length; arr.size
来源：http://le.huanxung.cn

C#:   list.Count;
来源：http://fg.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://as.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yx.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wm.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://sv.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://rg.521024.cn

Java: list.subList(1, 4);
来源：http://jg.panjiajie.cn

Go:   arr[1:4]
来源：http://sc.shxzukj.cn

Ruby: arr[1, 3]
来源：http://nv.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://aw.hahajie.cn

[D08] 合并两个数组
来源：http://mt.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ha.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://ki.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nw.jctech888.com.cn

TS:   [...a, ...b];
来源：http://nb.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cc.haigaiapp.cn

Go:   append(a, b...)
来源：http://ou.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://uf.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://mi.colortex.cn

[D09] 排序（升序）
来源：http://ka.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.szsharing.cn

PHP:  sort($arr);
来源：http://jw.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ku.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bh.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rq.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lm.shxzukj.cn

Ruby: arr.sort
来源：http://ey.chemitech.net.cn

C#:   list.Sort();
来源：http://ca.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fl.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tf.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lw.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pf.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qq.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://co.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cl.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dy.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ht.shxzukj.cn

[D11] 反转数组
来源：http://wu.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://un.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://tt.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ot.nicolike.cn

TS:   [...arr].reverse();
来源：http://zs.huanxung.cn

Java: Collections.reverse(list);
来源：http://za.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://qs.huixiangedu.cn

Ruby: arr.reverse
来源：http://zi.bookmarksfly.cn

C#:   list.Reverse();
来源：http://qr.nicolike.cn

[D12] 查找元素下标
来源：http://vb.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://gc.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kg.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dd.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kp.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zd.colortex.cn

Go:   slices.Index(arr, x)
来源：http://dc.nicolike.cn

Ruby: arr.index(x)
来源：http://vf.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://eh.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://xw.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bf.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cy.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://so.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ey.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://if.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zd.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kw.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kc.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://jh.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ph.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bi.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://or.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://xn.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ez.asd995.cn

Go:   // 手写循环
来源：http://od.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qt.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ls.wgjwhj.cn

[D15] 去重
来源：http://xy.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vl.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://es.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://ov.jianghongdianzi.cn


<!-- 参考信息 -->