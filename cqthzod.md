代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ut.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bk.newstarts.cn

[B15] 布尔运算与取反
来源：http://xc.haigaiapp.cn

Py:   a and b or not c
来源：http://hq.colortex.cn

PHP:  $a && $b || !$c
来源：http://ec.yuexingan06.cn

JS:   a && b || !c
来源：http://vk.wgjwhj.cn

TS:   a && b || !c
来源：http://nv.jianghongdianzi.cn

Java: a && b || !c
来源：http://ir.nicolike.cn

Go:   a && b || !c
来源：http://nn.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://as.haigaiapp.cn

C#:   a && b || !c
来源：http://uo.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vc.jctech888.com.cn

Py:   if not data: return
来源：http://lc.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://bd.hahajie.cn

JS:   if (!data) return;
来源：http://sy.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://br.panjiajie.cn

Java: if (data == null) return;
来源：http://ve.nszjky.cn

Go:   if data == nil { return }
来源：http://hx.colortex.cn

Ruby: return if data.nil?
来源：http://ov.shxzskj.cn

C#:   if (data == null) return;
来源：http://of.shxzskj.cn

================================================================================
来源：http://yy.hahajie.cn

C. 函数与作用域
来源：http://gm.wgjwhj.cn

================================================================================
来源：http://cw.huanxung.cn

[C01] 定义函数
来源：http://ww.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://yw.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ik.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://de.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bh.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qi.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kh.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://kq.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bl.shxzskj.cn

[C02] 默认参数
来源：http://zh.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://sc.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gt.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://ha.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xa.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://or.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jl.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://qg.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://bx.newstarts.cn

[C03] 可变参数
来源：http://bl.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://kx.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ov.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bb.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qc.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uu.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wv.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://an.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zn.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://rm.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gw.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jv.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://az.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xl.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ij.521024.cn

Go:   // 无：用配置结构体参数
来源：http://cz.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://wv.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://jh.9csxet.cn

[C05] 返回多个值
来源：http://hm.nszjky.cn

Py:   return a, b
来源：http://bq.9csxet.cn

PHP:  return [$a, $b];
来源：http://yu.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xq.chemitech.net.cn

TS:   return { a, b };
来源：http://ue.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jh.shxzskj.cn

Go:   return a, b
来源：http://od.muxihuayi.cn

Ruby: return a, b
来源：http://ex.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://yd.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://qn.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://wi.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://on.huanxung.cn

JS:   const square = x => x * x;
来源：http://xh.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://fg.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kb.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uj.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://cu.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oq.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://cj.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ii.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mc.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kn.nszjky.cn

TS:   arr.map(String)
来源：http://xy.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jk.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://us.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://or.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gz.colortex.cn

[C08] 闭包
来源：http://wo.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hq.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mt.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xy.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gp.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ub.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cq.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zr.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jd.colortex.cn

[C09] 递归
来源：http://eo.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://je.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ul.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://if.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://er.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bo.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dd.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ex.huixiangedu.cn

[C10] 变量作用域
来源：http://qs.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gt.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iz.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fn.521024.cn

TS:   同 JS
来源：http://az.szsharing.cn

Java: 方法内为块级作用域
来源：http://hl.panjiajie.cn

Go:   花括号块级作用域
来源：http://rx.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vy.jctech888.com.cn

C#:   块级作用域
来源：http://dj.huixiangedu.cn

[C11] 模块导入与导出
来源：http://an.nicolike.cn

Py:   from module import func
来源：http://dx.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mq.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dk.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vr.panjiajie.cn

Java: import java.util.List;
来源：http://xh.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nm.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://cp.521024.cn

C#:   using System.Text;
来源：http://ut.521024.cn

[C12] 立即执行函数 IIFE
来源：http://vb.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://yn.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://sj.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://mk.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://gv.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://at.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://fk.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://gm.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cr.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://rv.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ep.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kr.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://va.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tc.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pj.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://uz.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nm.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kx.bookmarksfly.cn

[C14] 泛型函数
来源：http://ne.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://te.panjiajie.cn

PHP:  // 无泛型
来源：http://en.haigaiapp.cn

JS:   // 无泛型
来源：http://de.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://av.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gk.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jr.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://lh.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ss.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://qj.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bq.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://dp.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tr.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ai.wgjwhj.cn

Java: // 无解构
来源：http://jd.colortex.cn

Go:   // 无解构
来源：http://cj.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://ci.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://fm.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://jn.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xk.muxihuayi.cn

PHP:  // 无重载
来源：http://bc.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ah.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://qp.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lw.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://dk.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://qb.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ge.lnxyls.cn

================================================================================
来源：http://ha.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://uf.yuntaijiaju.cn

================================================================================
来源：http://zs.nicolike.cn

[D01] 创建数组 / 列表
来源：http://ni.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tb.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eb.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cu.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cx.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tq.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://cu.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://zd.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.szxytkj.cn

[D02] 追加元素到末尾
来源：http://qe.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ic.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ly.shxzskj.cn

JS:   arr.push(4);
来源：http://iv.szxytkj.cn

TS:   arr.push(4);
来源：http://bi.colortex.cn

Java: list.add(4);
来源：http://yj.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://pi.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://xr.colortex.cn

C#:   list.Add(4);
来源：http://ka.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ry.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://yq.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ou.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lr.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://qn.shtwfgs.cn

Java: list.add(0, 0);
来源：http://al.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://br.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fa.asd995.cn

C#:   list.Insert(0, 0);
来源：http://lo.yuexingan06.cn

[D04] 删除元素
来源：http://ge.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cd.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rg.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dt.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://we.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rt.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vd.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eo.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kl.9csxet.cn

[D05] 访问与修改元素
来源：http://vw.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dk.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://we.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qc.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://do.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://va.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://lb.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jq.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tm.yuexingan06.cn

[D06] 数组长度
来源：http://bc.jctech888.com.cn

Py:   len(arr)
来源：http://bq.chemitech.net.cn

PHP:  count($arr);
来源：http://gk.yuexingan06.cn

JS:   arr.length
来源：http://ef.bjjhwx.cn

TS:   arr.length
来源：http://ty.jianghongdianzi.cn

Java: list.size();
来源：http://kh.bjjhwx.cn

Go:   len(arr)
来源：http://sq.hahajie.cn

Ruby: arr.length; arr.size
来源：http://rx.bjjhwx.cn

C#:   list.Count;
来源：http://dk.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://ue.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hu.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://og.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://ha.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://my.lnxyls.cn

Java: list.subList(1, 4);
来源：http://xo.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://fz.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ls.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://gd.newstarts.cn

[D08] 合并两个数组
来源：http://pk.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://qw.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://vk.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bi.shxzukj.cn

TS:   [...a, ...b];
来源：http://ux.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bp.szsharing.cn

Go:   append(a, b...)
来源：http://xd.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://th.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://fx.nszjky.cn

[D09] 排序（升序）
来源：http://mj.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://lz.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yk.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ie.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aa.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ok.gzmigu.cn

Ruby: arr.sort
来源：http://ag.gzmigu.cn

C#:   list.Sort();
来源：http://ao.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xk.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rt.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tj.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bt.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pr.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bm.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bb.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uj.haigaiapp.cn

[D11] 反转数组
来源：http://bg.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cd.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://bp.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bm.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://cp.nicolike.cn

Java: Collections.reverse(list);
来源：http://gq.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://ev.hnjuh.cn

Ruby: arr.reverse
来源：http://ph.asd995.cn

C#:   list.Reverse();
来源：http://jl.colortex.cn

[D12] 查找元素下标
来源：http://hw.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://cl.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://va.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gr.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lw.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cn.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://bq.nicolike.cn

Ruby: arr.index(x)
来源：http://ge.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://mq.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://tb.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aw.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ym.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://cc.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://sx.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jf.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nh.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xg.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jm.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://pd.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nl.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fl.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://df.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://yo.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zc.521024.cn

Go:   // 手写循环
来源：http://sh.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hp.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://an.hahajie.cn

[D15] 去重
来源：http://zq.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hu.gzmigu.cn

PHP:  array_unique($arr);
来源：http://kx.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://sl.gzmigu.cn


<!-- 参考信息 -->