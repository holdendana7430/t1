代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://td.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://iw.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cj.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ot.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jn.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://di.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ac.shtwfgs.cn

Py:   a and b or not c
来源：http://vp.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://dy.nszjky.cn

JS:   a && b || !c
来源：http://oc.newstarts.cn

TS:   a && b || !c
来源：http://tx.jianghongdianzi.cn

Java: a && b || !c
来源：http://dj.9csxet.cn

Go:   a && b || !c
来源：http://in.yuexingan06.cn

Ruby: a && b || !c
来源：http://zd.hnjuh.cn

C#:   a && b || !c
来源：http://fx.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nw.chemitech.net.cn

Py:   if not data: return
来源：http://xc.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://ef.gzmigu.cn

JS:   if (!data) return;
来源：http://xs.muxihuayi.cn

TS:   if (!data) return;
来源：http://ts.shtwfgs.cn

Java: if (data == null) return;
来源：http://ls.gzmigu.cn

Go:   if data == nil { return }
来源：http://fr.nszjky.cn

Ruby: return if data.nil?
来源：http://ja.lnxyls.cn

C#:   if (data == null) return;
来源：http://za.szsharing.cn

================================================================================
来源：http://df.panjiajie.cn

C. 函数与作用域
来源：http://ua.szxytkj.cn

================================================================================
来源：http://yq.bjjhwx.cn

[C01] 定义函数
来源：http://zt.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://xv.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://el.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://cb.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hl.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vh.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://it.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://jw.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lv.newstarts.cn

[C02] 默认参数
来源：http://qw.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://bu.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hq.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ix.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oj.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qy.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://qg.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://fx.yuexingan06.cn

[C03] 可变参数
来源：http://up.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://od.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rb.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jj.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ey.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uu.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zl.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cn.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://vs.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ft.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zu.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://af.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ls.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://il.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://sm.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://hi.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://qv.jianghongdianzi.cn

[C05] 返回多个值
来源：http://mr.yuntaijiaju.cn

Py:   return a, b
来源：http://ri.shxzskj.cn

PHP:  return [$a, $b];
来源：http://ti.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qc.jctech888.com.cn

TS:   return { a, b };
来源：http://px.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mr.newstarts.cn

Go:   return a, b
来源：http://py.chemitech.net.cn

Ruby: return a, b
来源：http://dj.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://oe.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://eo.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://lq.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oh.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://fr.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://aj.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uj.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hu.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://qx.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kp.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://if.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jq.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://di.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ml.yuexingan06.cn

TS:   arr.map(String)
来源：http://eo.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ak.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iz.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://md.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mh.szsharing.cn

[C08] 闭包
来源：http://tp.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ag.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://md.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ah.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nt.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kw.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xf.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://or.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vq.newstarts.cn

[C09] 递归
来源：http://sd.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ti.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qy.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://in.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wb.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ge.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gz.huanxung.cn

[C10] 变量作用域
来源：http://qm.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fm.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nl.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qh.newstarts.cn

TS:   同 JS
来源：http://mp.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://xe.hahajie.cn

Go:   花括号块级作用域
来源：http://ld.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zu.szsharing.cn

C#:   块级作用域
来源：http://ag.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ii.haigaiapp.cn

Py:   from module import func
来源：http://aw.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gb.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ox.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uc.bookmarksfly.cn

Java: import java.util.List;
来源：http://kc.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://li.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://fw.bookmarksfly.cn

C#:   using System.Text;
来源：http://hp.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://ur.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://au.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://sy.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://fy.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ad.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hy.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://dv.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://dc.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://we.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://xt.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ru.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nq.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rp.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://am.nicolike.cn

Go:   func add(a, b int) int
来源：http://ae.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yp.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cd.yuexingan06.cn

[C14] 泛型函数
来源：http://or.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://td.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://xf.newstarts.cn

JS:   // 无泛型
来源：http://uy.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xg.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fu.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wm.huixiangedu.cn

Ruby: # 无泛型
来源：http://rn.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dr.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://cq.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cv.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://qx.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://se.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sq.wgjwhj.cn

Java: // 无解构
来源：http://hu.nszjky.cn

Go:   // 无解构
来源：http://vy.asd995.cn

Ruby: a, b = pair
来源：http://ku.asd995.cn

C#:   var (a, b) = pair;
来源：http://kl.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://xw.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ry.nicolike.cn

PHP:  // 无重载
来源：http://bx.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nl.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://br.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sn.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://ob.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://zy.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://au.szxytkj.cn

================================================================================
来源：http://fw.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://yg.yuexingan06.cn

================================================================================
来源：http://sf.colortex.cn

[D01] 创建数组 / 列表
来源：http://hp.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oc.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fd.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ga.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sy.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://td.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://yl.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://jo.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://py.521024.cn

[D02] 追加元素到末尾
来源：http://mu.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ji.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tp.gzmigu.cn

JS:   arr.push(4);
来源：http://yu.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://fu.muxihuayi.cn

Java: list.add(4);
来源：http://lh.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://oz.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://vo.panjiajie.cn

C#:   list.Add(4);
来源：http://gd.nicolike.cn

[D03] 在指定位置插入元素
来源：http://em.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://hw.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jg.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oy.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://da.hnjuh.cn

Java: list.add(0, 0);
来源：http://bj.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hh.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zq.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://qp.wgjwhj.cn

[D04] 删除元素
来源：http://sr.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hj.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://px.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pd.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ry.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ap.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bc.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ow.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fu.shtwfgs.cn

[D05] 访问与修改元素
来源：http://ni.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ec.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xr.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ph.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://qa.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://rw.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ya.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dn.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bb.jctech888.com.cn

[D06] 数组长度
来源：http://rm.asd995.cn

Py:   len(arr)
来源：http://vu.shxzskj.cn

PHP:  count($arr);
来源：http://hs.newstarts.cn

JS:   arr.length
来源：http://dv.shxzskj.cn

TS:   arr.length
来源：http://ej.shxzskj.cn

Java: list.size();
来源：http://we.colortex.cn

Go:   len(arr)
来源：http://gf.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://yv.shxzukj.cn

C#:   list.Count;
来源：http://az.huanxung.cn

[D07] 切片 / 取子数组
来源：http://li.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oa.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qv.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://cv.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://yj.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://dj.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ju.colortex.cn

Ruby: arr[1, 3]
来源：http://vy.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://dj.asd995.cn

[D08] 合并两个数组
来源：http://sw.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://yg.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://qe.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ep.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://gp.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pe.bjjhwx.cn

Go:   append(a, b...)
来源：http://hv.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://et.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://pm.huixiangedu.cn

[D09] 排序（升序）
来源：http://bt.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://gz.panjiajie.cn

PHP:  sort($arr);
来源：http://uo.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tb.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wt.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xe.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hj.szxytkj.cn

Ruby: arr.sort
来源：http://co.gzmigu.cn

C#:   list.Sort();
来源：http://we.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ft.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qx.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cs.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sv.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ra.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ri.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://it.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bm.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://os.bookmarksfly.cn

[D11] 反转数组
来源：http://gm.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wf.nszjky.cn

PHP:  array_reverse($arr);
来源：http://dr.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ss.huanxung.cn

TS:   [...arr].reverse();
来源：http://kf.nszjky.cn

Java: Collections.reverse(list);
来源：http://ys.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://el.bjjhwx.cn

Ruby: arr.reverse
来源：http://or.nszjky.cn

C#:   list.Reverse();
来源：http://se.chemitech.net.cn

[D12] 查找元素下标
来源：http://so.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://gu.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ch.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uo.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fi.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qb.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://zj.lnxyls.cn

Ruby: arr.index(x)
来源：http://pp.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://rv.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://nr.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ai.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://te.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://mm.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://zh.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zu.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yh.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xm.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cj.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://jf.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cp.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fy.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://zq.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://ae.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fr.huixinmuqiang.cn

Go:   // 手写循环
来源：http://zn.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dh.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://im.bookmarksfly.cn


<!-- 参考信息 -->