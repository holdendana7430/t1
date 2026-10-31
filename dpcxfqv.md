代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gd.jianghongdianzi.cn

Java: x instanceof Number
来源：http://bh.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://op.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://tx.colortex.cn

C#:   x is int or double or decimal
来源：http://yv.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://iv.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ex.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hf.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://jy.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://oh.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ez.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lk.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ar.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ll.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://pv.shxzskj.cn

Py:   a and b or not c
来源：http://kb.huanxung.cn

PHP:  $a && $b || !$c
来源：http://ea.gzmigu.cn

JS:   a && b || !c
来源：http://fb.gzmigu.cn

TS:   a && b || !c
来源：http://ec.bookmarksfly.cn

Java: a && b || !c
来源：http://jb.nszjky.cn

Go:   a && b || !c
来源：http://vc.yuexingan06.cn

Ruby: a && b || !c
来源：http://kx.shxzukj.cn

C#:   a && b || !c
来源：http://jn.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uj.shxzskj.cn

Py:   if not data: return
来源：http://ue.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://fw.lnxyls.cn

JS:   if (!data) return;
来源：http://jv.huixiangedu.cn

TS:   if (!data) return;
来源：http://hf.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://vt.asd995.cn

Go:   if data == nil { return }
来源：http://uh.wgjwhj.cn

Ruby: return if data.nil?
来源：http://ym.szsharing.cn

C#:   if (data == null) return;
来源：http://ef.wgjwhj.cn

================================================================================
来源：http://eb.shtwfgs.cn

C. 函数与作用域
来源：http://cg.huanxung.cn

================================================================================
来源：http://pw.newstarts.cn

[C01] 定义函数
来源：http://da.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://gu.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ei.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://rj.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ih.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xd.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fm.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://wc.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lg.lnxyls.cn

[C02] 默认参数
来源：http://gz.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://kh.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dt.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://xu.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ia.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cj.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vb.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://wf.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ef.shtwfgs.cn

[C03] 可变参数
来源：http://eu.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://dz.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yy.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hb.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zj.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dr.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nu.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rv.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://pk.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pw.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jd.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lz.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://es.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://db.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://kb.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://vg.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://hq.shxzukj.cn

[C05] 返回多个值
来源：http://jz.9csxet.cn

Py:   return a, b
来源：http://vh.newstarts.cn

PHP:  return [$a, $b];
来源：http://hh.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dp.wgjwhj.cn

TS:   return { a, b };
来源：http://kn.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://co.jianghongdianzi.cn

Go:   return a, b
来源：http://ve.9csxet.cn

Ruby: return a, b
来源：http://bp.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ce.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://vr.huanxung.cn

Py:   square = lambda x: x * x
来源：http://an.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ki.huanxung.cn

JS:   const square = x => x * x;
来源：http://ps.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://jw.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nb.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uo.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://bz.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vh.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://ct.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rr.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ws.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zx.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://vh.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ey.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bb.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://jy.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://re.asd995.cn

[C08] 闭包
来源：http://cw.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ai.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yw.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cp.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qt.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vy.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zg.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zu.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aq.wgjwhj.cn

[C09] 递归
来源：http://sj.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://io.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fn.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sj.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://od.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cj.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://is.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sz.huixiangedu.cn

[C10] 变量作用域
来源：http://qn.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fv.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://br.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bc.huixinmuqiang.cn

TS:   同 JS
来源：http://zm.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://su.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://le.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nc.colortex.cn

C#:   块级作用域
来源：http://xg.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://dh.jctech888.com.cn

Py:   from module import func
来源：http://fd.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xq.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sd.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ya.bjjhwx.cn

Java: import java.util.List;
来源：http://wu.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vz.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://sg.yuntaijiaju.cn

C#:   using System.Text;
来源：http://ht.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://de.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://vh.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ww.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://ow.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://nc.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sj.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://xd.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://on.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uy.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://lt.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hu.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kr.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uv.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cv.asd995.cn

Go:   func add(a, b int) int
来源：http://vj.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gn.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://co.bookmarksfly.cn

[C14] 泛型函数
来源：http://en.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sd.asd995.cn

PHP:  // 无泛型
来源：http://jl.newstarts.cn

JS:   // 无泛型
来源：http://di.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sx.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xl.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gj.9csxet.cn

Ruby: # 无泛型
来源：http://li.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mk.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://zo.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qa.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://br.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rq.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lb.colortex.cn

Java: // 无解构
来源：http://tu.colortex.cn

Go:   // 无解构
来源：http://ln.nicolike.cn

Ruby: a, b = pair
来源：http://vn.asd995.cn

C#:   var (a, b) = pair;
来源：http://ls.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://di.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xn.hahajie.cn

PHP:  // 无重载
来源：http://bn.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mp.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://hr.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lx.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://dm.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://pu.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://km.hnjuh.cn

================================================================================
来源：http://td.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://gb.muxihuayi.cn

================================================================================
来源：http://rr.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://fz.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ks.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eb.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://so.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ot.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tv.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://eu.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://ce.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://he.panjiajie.cn

[D02] 追加元素到末尾
来源：http://qy.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ny.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tm.yuexingan06.cn

JS:   arr.push(4);
来源：http://rx.wgjwhj.cn

TS:   arr.push(4);
来源：http://uw.bjjhwx.cn

Java: list.add(4);
来源：http://pt.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://vi.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ov.521024.cn

C#:   list.Add(4);
来源：http://xs.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://fl.colortex.cn

Py:   arr.insert(0, 0)
来源：http://ap.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nc.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wj.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://in.asd995.cn

Java: list.add(0, 0);
来源：http://qw.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tt.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uy.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://uc.panjiajie.cn

[D04] 删除元素
来源：http://uf.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://br.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mi.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ze.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://kr.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dn.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fq.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ex.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lo.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://nh.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://al.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sf.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ud.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://jl.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://sl.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://km.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fr.wgjwhj.cn

[D06] 数组长度
来源：http://gl.yuntaijiaju.cn

Py:   len(arr)
来源：http://sd.huixiangedu.cn

PHP:  count($arr);
来源：http://da.colortex.cn

JS:   arr.length
来源：http://lc.shtwfgs.cn

TS:   arr.length
来源：http://zx.wgjwhj.cn

Java: list.size();
来源：http://ry.hnjuh.cn

Go:   len(arr)
来源：http://cv.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://vv.9csxet.cn

C#:   list.Count;
来源：http://yu.9csxet.cn

[D07] 切片 / 取子数组
来源：http://iu.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hh.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ki.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://tu.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://lg.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://sv.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ps.hnjuh.cn

Ruby: arr[1, 3]
来源：http://mi.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://hn.asd995.cn

[D08] 合并两个数组
来源：http://va.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://wb.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://gd.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ap.jctech888.com.cn

TS:   [...a, ...b];
来源：http://wc.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ec.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://hb.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://xi.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://uq.hahajie.cn

[D09] 排序（升序）
来源：http://sy.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.521024.cn

PHP:  sort($arr);
来源：http://xv.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://we.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mf.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mw.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hd.nszjky.cn

Ruby: arr.sort
来源：http://bj.szsharing.cn

C#:   list.Sort();
来源：http://ig.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vo.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dy.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://di.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gx.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rf.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eb.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dm.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://to.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qe.jctech888.com.cn

[D11] 反转数组
来源：http://pn.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ka.hahajie.cn

PHP:  array_reverse($arr);
来源：http://xa.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vy.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://em.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://xw.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://fj.gzmigu.cn

Ruby: arr.reverse
来源：http://zo.huixiangedu.cn

C#:   list.Reverse();
来源：http://tm.wgjwhj.cn

[D12] 查找元素下标
来源：http://fe.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://xt.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://of.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fh.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rb.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xe.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://nm.9csxet.cn

Ruby: arr.index(x)
来源：http://yd.521024.cn

C#:   list.IndexOf(x);
来源：http://qt.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://gs.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bv.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xe.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://gc.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://jz.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hl.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gc.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eu.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://pe.hnjuh.cn


<!-- 参考信息 -->