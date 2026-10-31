代发 wailian999

[B13] 判断是否为数字
来源：http://sd.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://sh.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://dw.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gw.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dw.9csxet.cn

Java: x instanceof Number
来源：http://wp.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ql.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://ph.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://uq.szsharing.cn

[B14] 判断值是否在集合内
来源：http://so.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qd.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://hs.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://hy.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vz.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://px.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://it.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ck.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ds.wgjwhj.cn

Py:   a and b or not c
来源：http://qc.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://xj.shxzukj.cn

JS:   a && b || !c
来源：http://jp.haigaiapp.cn

TS:   a && b || !c
来源：http://bg.jianghongdianzi.cn

Java: a && b || !c
来源：http://yl.jctech888.com.cn

Go:   a && b || !c
来源：http://so.panjiajie.cn

Ruby: a && b || !c
来源：http://zz.szsharing.cn

C#:   a && b || !c
来源：http://tz.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gh.szsharing.cn

Py:   if not data: return
来源：http://sg.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://av.huanxung.cn

JS:   if (!data) return;
来源：http://fr.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://kq.nicolike.cn

Java: if (data == null) return;
来源：http://ed.lnxyls.cn

Go:   if data == nil { return }
来源：http://yk.huanxung.cn

Ruby: return if data.nil?
来源：http://hy.shxzukj.cn

C#:   if (data == null) return;
来源：http://sk.asd995.cn

================================================================================
来源：http://mo.bookmarksfly.cn

C. 函数与作用域
来源：http://xq.bookmarksfly.cn

================================================================================
来源：http://cp.9csxet.cn

[C01] 定义函数
来源：http://gi.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://qo.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ea.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://yo.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tp.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wm.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eb.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://le.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ez.nszjky.cn

[C02] 默认参数
来源：http://qu.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://mt.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://cv.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nj.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gj.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bl.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://fk.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hg.9csxet.cn

[C03] 可变参数
来源：http://vk.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://qq.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ix.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vl.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ou.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jl.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ot.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bf.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cs.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://up.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jb.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://un.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yv.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hk.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://un.521024.cn

Go:   // 无：用配置结构体参数
来源：http://nt.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ks.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://cu.yuexingan06.cn

[C05] 返回多个值
来源：http://tq.jianghongdianzi.cn

Py:   return a, b
来源：http://un.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://ls.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ha.9csxet.cn

TS:   return { a, b };
来源：http://dc.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sg.lnxyls.cn

Go:   return a, b
来源：http://rz.nicolike.cn

Ruby: return a, b
来源：http://xn.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://hk.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pa.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://tk.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ef.szsharing.cn

JS:   const square = x => x * x;
来源：http://jp.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://el.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pp.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pl.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://mw.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dc.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://xs.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sh.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://an.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lx.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://po.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://na.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://id.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hc.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wr.nicolike.cn

[C08] 闭包
来源：http://qv.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ik.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ki.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jw.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pu.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vi.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://np.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cy.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gk.shtwfgs.cn

[C09] 递归
来源：http://bz.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sm.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rp.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qj.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://np.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kg.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ev.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ho.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uq.huanxung.cn

[C10] 变量作用域
来源：http://zn.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://je.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ig.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cp.colortex.cn

TS:   同 JS
来源：http://gk.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://dl.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://rj.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tj.chemitech.net.cn

C#:   块级作用域
来源：http://ni.bjjhwx.cn

[C11] 模块导入与导出
来源：http://fq.hnjuh.cn

Py:   from module import func
来源：http://ap.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ta.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xf.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pb.szsharing.cn

Java: import java.util.List;
来源：http://rr.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rx.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://bn.yuexingan06.cn

C#:   using System.Text;
来源：http://zq.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://zf.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://bv.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://py.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://sb.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://uk.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rf.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://gj.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ee.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xj.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://jy.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gr.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tb.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bk.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rc.colortex.cn

Go:   func add(a, b int) int
来源：http://pl.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bp.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sv.yuexingan06.cn

[C14] 泛型函数
来源：http://zq.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wm.shxzukj.cn

PHP:  // 无泛型
来源：http://qc.bjjhwx.cn

JS:   // 无泛型
来源：http://az.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cn.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fs.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qv.nszjky.cn

Ruby: # 无泛型
来源：http://ue.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bx.newstarts.cn

[C15] 解构 / 展开参数
来源：http://ky.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xk.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://jb.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mz.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vk.newstarts.cn

Java: // 无解构
来源：http://ay.gzmigu.cn

Go:   // 无解构
来源：http://xv.shxzukj.cn

Ruby: a, b = pair
来源：http://el.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://yl.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ad.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fq.gzmigu.cn

PHP:  // 无重载
来源：http://kq.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jp.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://dy.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jm.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://qv.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://fk.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fp.shxzukj.cn

================================================================================
来源：http://pe.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://ig.huixiangedu.cn

================================================================================
来源：http://ai.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://xj.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fd.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pl.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mk.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zi.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://po.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://da.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://wr.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eg.521024.cn

[D02] 追加元素到末尾
来源：http://nz.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ks.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zl.shxzskj.cn

JS:   arr.push(4);
来源：http://tu.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://nl.nszjky.cn

Java: list.add(4);
来源：http://nr.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://zh.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ti.lnxyls.cn

C#:   list.Add(4);
来源：http://tc.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://ee.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://iv.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://db.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://og.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://yx.huanxung.cn

Java: list.add(0, 0);
来源：http://ju.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xm.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yy.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://pa.lnxyls.cn

[D04] 删除元素
来源：http://oq.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ud.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uf.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ex.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cg.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://di.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://is.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lx.asd995.cn

[D05] 访问与修改元素
来源：http://uw.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kh.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hb.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gn.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://sp.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://as.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://uo.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ad.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gf.bookmarksfly.cn

[D06] 数组长度
来源：http://tt.bjjhwx.cn

Py:   len(arr)
来源：http://cq.haigaiapp.cn

PHP:  count($arr);
来源：http://gd.jianghongdianzi.cn

JS:   arr.length
来源：http://aw.gzmigu.cn

TS:   arr.length
来源：http://yl.haigaiapp.cn

Java: list.size();
来源：http://so.jianghongdianzi.cn

Go:   len(arr)
来源：http://qk.szsharing.cn

Ruby: arr.length; arr.size
来源：http://bf.asd995.cn

C#:   list.Count;
来源：http://qg.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://bm.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ly.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jh.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://yc.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://zj.panjiajie.cn

Java: list.subList(1, 4);
来源：http://oc.bjjhwx.cn

Go:   arr[1:4]
来源：http://rq.shxzskj.cn

Ruby: arr[1, 3]
来源：http://nj.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://op.bjjhwx.cn

[D08] 合并两个数组
来源：http://lz.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://vt.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://yb.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gu.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ev.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kz.lnxyls.cn

Go:   append(a, b...)
来源：http://vv.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://vk.521024.cn

C#:   a.Concat(b).ToList()
来源：http://gm.shxzukj.cn

[D09] 排序（升序）
来源：http://np.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.521024.cn

PHP:  sort($arr);
来源：http://ya.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cc.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://us.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zm.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ue.shtwfgs.cn

Ruby: arr.sort
来源：http://jn.huixiangedu.cn

C#:   list.Sort();
来源：http://jh.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lb.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bf.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://br.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vx.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://us.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jz.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rx.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lu.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fc.huixiangedu.cn

[D11] 反转数组
来源：http://nd.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ad.hahajie.cn

PHP:  array_reverse($arr);
来源：http://uw.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ru.newstarts.cn

TS:   [...arr].reverse();
来源：http://lm.szxytkj.cn

Java: Collections.reverse(list);
来源：http://eb.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://vq.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://mf.huanxung.cn

C#:   list.Reverse();
来源：http://tu.shtwfgs.cn

[D12] 查找元素下标
来源：http://qq.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://rm.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kb.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xb.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vv.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dk.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://pk.bjjhwx.cn

Ruby: arr.index(x)
来源：http://vr.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://oh.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://ad.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nv.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ok.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://jy.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://cs.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dc.lnxyls.cn


<!-- 参考信息 -->