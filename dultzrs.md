代发 wailian999

PHP:  $a && $b || !$c
来源：http://im.huixiangedu.cn

JS:   a && b || !c
来源：http://id.gzmigu.cn

TS:   a && b || !c
来源：http://wg.bjjhwx.cn

Java: a && b || !c
来源：http://uc.colortex.cn

Go:   a && b || !c
来源：http://oq.lnxyls.cn

Ruby: a && b || !c
来源：http://hi.asd995.cn

C#:   a && b || !c
来源：http://mk.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jm.gzmigu.cn

Py:   if not data: return
来源：http://iv.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://fu.nszjky.cn

JS:   if (!data) return;
来源：http://zl.lnxyls.cn

TS:   if (!data) return;
来源：http://or.huixiangedu.cn

Java: if (data == null) return;
来源：http://tv.shxzukj.cn

Go:   if data == nil { return }
来源：http://at.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ni.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://ey.asd995.cn

================================================================================
来源：http://uu.gzmigu.cn

C. 函数与作用域
来源：http://ta.bookmarksfly.cn

================================================================================
来源：http://jd.521024.cn

[C01] 定义函数
来源：http://xg.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://it.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://mk.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://to.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://an.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gh.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://xy.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ie.colortex.cn

[C02] 默认参数
来源：http://wb.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://gt.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mx.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ek.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fh.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pn.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kl.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://lt.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://fe.szsharing.cn

[C03] 可变参数
来源：http://iw.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ka.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aw.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hc.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nf.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lr.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sk.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uw.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jb.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://wg.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tg.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ta.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kl.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://td.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://cu.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://wf.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://cr.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://of.jianghongdianzi.cn

[C05] 返回多个值
来源：http://kj.szsharing.cn

Py:   return a, b
来源：http://hr.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://vz.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ay.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ey.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xv.jianghongdianzi.cn

Go:   return a, b
来源：http://pl.huanxung.cn

Ruby: return a, b
来源：http://gc.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://jj.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://zh.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://nu.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vr.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ra.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://fm.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dg.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pq.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://vi.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bj.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://rk.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fn.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xx.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gm.gzmigu.cn

TS:   arr.map(String)
来源：http://zw.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aw.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ht.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://ie.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ax.yuntaijiaju.cn

[C08] 闭包
来源：http://bn.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://in.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uz.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yg.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qi.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ly.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ig.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xf.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dk.huanxung.cn

[C09] 递归
来源：http://qr.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mj.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lu.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ea.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dk.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vh.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rv.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vu.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yt.newstarts.cn

[C10] 变量作用域
来源：http://rq.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tr.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pb.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gg.panjiajie.cn

TS:   同 JS
来源：http://ba.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ow.szxytkj.cn

Go:   花括号块级作用域
来源：http://qj.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gi.huanxung.cn

C#:   块级作用域
来源：http://xl.panjiajie.cn

[C11] 模块导入与导出
来源：http://di.colortex.cn

Py:   from module import func
来源：http://iv.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wb.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oy.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uk.jianghongdianzi.cn

Java: import java.util.List;
来源：http://bv.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://km.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://bh.521024.cn

C#:   using System.Text;
来源：http://ga.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://ph.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://bn.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ok.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://uo.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://bi.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gx.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nq.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ya.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bg.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://jl.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tl.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ht.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://te.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yj.shxzskj.cn

Go:   func add(a, b int) int
来源：http://qm.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ck.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mx.shxzukj.cn

[C14] 泛型函数
来源：http://ne.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kt.huixiangedu.cn

PHP:  // 无泛型
来源：http://mg.yuexingan06.cn

JS:   // 无泛型
来源：http://dn.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://os.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gu.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://up.9csxet.cn

Ruby: # 无泛型
来源：http://pe.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ze.szsharing.cn

[C15] 解构 / 展开参数
来源：http://de.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vc.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://zr.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://we.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wo.bjjhwx.cn

Java: // 无解构
来源：http://po.colortex.cn

Go:   // 无解构
来源：http://bu.shxzukj.cn

Ruby: a, b = pair
来源：http://sv.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://by.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://vq.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ar.shxzskj.cn

PHP:  // 无重载
来源：http://wf.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mi.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://kb.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wc.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://gq.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://wy.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sv.haigaiapp.cn

================================================================================
来源：http://ng.521024.cn

D. 数组 / 列表 / 集合
来源：http://pt.huixinmuqiang.cn

================================================================================
来源：http://gi.nszjky.cn

[D01] 创建数组 / 列表
来源：http://tc.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mb.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hi.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nd.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zw.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dw.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://fw.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://ah.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ni.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://hk.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uu.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tk.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://pn.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://rv.chemitech.net.cn

Java: list.add(4);
来源：http://oj.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://kb.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://wc.shtwfgs.cn

C#:   list.Add(4);
来源：http://rh.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://la.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://ra.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gw.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mz.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://sy.bjjhwx.cn

Java: list.add(0, 0);
来源：http://mx.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vb.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://ul.bookmarksfly.cn

[D04] 删除元素
来源：http://cb.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ij.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wg.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dy.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://qk.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ty.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aj.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ir.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xq.shxzukj.cn

[D05] 访问与修改元素
来源：http://ep.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rz.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eq.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gf.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://sj.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://qw.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://po.colortex.cn

[D06] 数组长度
来源：http://dc.szxytkj.cn

Py:   len(arr)
来源：http://dk.bookmarksfly.cn

PHP:  count($arr);
来源：http://vk.muxihuayi.cn

JS:   arr.length
来源：http://wh.jctech888.com.cn

TS:   arr.length
来源：http://wy.521024.cn

Java: list.size();
来源：http://si.lnxyls.cn

Go:   len(arr)
来源：http://qr.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://mv.panjiajie.cn

C#:   list.Count;
来源：http://tf.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://ny.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jr.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rr.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://tq.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://rq.521024.cn

Java: list.subList(1, 4);
来源：http://st.colortex.cn

Go:   arr[1:4]
来源：http://fo.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://xk.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://va.szxytkj.cn

[D08] 合并两个数组
来源：http://kd.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://ss.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://on.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rn.hnjuh.cn

TS:   [...a, ...b];
来源：http://jf.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ni.szxytkj.cn

Go:   append(a, b...)
来源：http://rd.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://yx.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://la.muxihuayi.cn

[D09] 排序（升序）
来源：http://ed.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://fa.shxzskj.cn

PHP:  sort($arr);
来源：http://oa.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ki.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rv.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://na.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zq.jianghongdianzi.cn

Ruby: arr.sort
来源：http://kn.yuexingan06.cn

C#:   list.Sort();
来源：http://mh.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://to.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qw.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pn.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qp.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://no.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pk.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rh.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tq.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://me.yuntaijiaju.cn

[D11] 反转数组
来源：http://un.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qq.colortex.cn

PHP:  array_reverse($arr);
来源：http://nq.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ra.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://iv.lnxyls.cn

Java: Collections.reverse(list);
来源：http://vc.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://yu.hnjuh.cn

Ruby: arr.reverse
来源：http://sw.shxzukj.cn

C#:   list.Reverse();
来源：http://yo.gzmigu.cn

[D12] 查找元素下标
来源：http://yl.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://wd.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iq.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ot.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yf.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vh.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://nm.hnjuh.cn

Ruby: arr.index(x)
来源：http://px.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://hb.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://wl.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jt.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vx.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://wh.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://rj.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jj.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ic.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://al.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kc.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://yw.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zz.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://as.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://tr.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://tb.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jb.muxihuayi.cn

Go:   // 手写循环
来源：http://ck.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kh.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.hnjuh.cn

[D15] 去重
来源：http://ys.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fk.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://mu.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://yg.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://wi.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bt.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xb.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://jg.shxzukj.cn


<!-- 参考信息 -->