代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://bb.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fj.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://uq.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iw.shxzskj.cn

[C02] 默认参数
来源：http://tx.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://ik.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cz.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://sz.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ut.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hl.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uu.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://lr.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://gl.chemitech.net.cn

[C03] 可变参数
来源：http://ef.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://wq.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ap.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fk.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tj.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yr.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nk.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zq.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wk.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://ol.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gm.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hd.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vg.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kr.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://vt.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://nd.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://lo.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://zp.jctech888.com.cn

[C05] 返回多个值
来源：http://lp.521024.cn

Py:   return a, b
来源：http://ee.szsharing.cn

PHP:  return [$a, $b];
来源：http://sz.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://st.shxzukj.cn

TS:   return { a, b };
来源：http://mx.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xw.asd995.cn

Go:   return a, b
来源：http://sh.panjiajie.cn

Ruby: return a, b
来源：http://we.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://mu.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://bt.nicolike.cn

Py:   square = lambda x: x * x
来源：http://xr.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ee.huanxung.cn

JS:   const square = x => x * x;
来源：http://sz.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://gk.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ta.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://me.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://do.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mz.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://jr.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nw.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ix.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yk.huanxung.cn

TS:   arr.map(String)
来源：http://jm.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vo.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ae.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://wz.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nd.jctech888.com.cn

[C08] 闭包
来源：http://dx.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dr.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gb.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ew.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bq.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xd.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ry.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xh.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rd.colortex.cn

[C09] 递归
来源：http://zm.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://io.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wv.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xa.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://al.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ie.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ue.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vy.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zw.szxytkj.cn

[C10] 变量作用域
来源：http://qc.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xz.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kq.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lc.bookmarksfly.cn

TS:   同 JS
来源：http://oe.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://nq.hnjuh.cn

Go:   花括号块级作用域
来源：http://ba.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jt.shtwfgs.cn

C#:   块级作用域
来源：http://pd.huanxung.cn

[C11] 模块导入与导出
来源：http://cd.wgjwhj.cn

Py:   from module import func
来源：http://in.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ga.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://et.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sc.jctech888.com.cn

Java: import java.util.List;
来源：http://or.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eo.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://uf.gzmigu.cn

C#:   using System.Text;
来源：http://xx.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://pf.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://lq.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://im.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://vs.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ap.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://at.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://rl.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://mb.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nw.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://uc.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qp.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://df.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qc.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tt.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://ht.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ir.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://go.shxzskj.cn

[C14] 泛型函数
来源：http://sw.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uq.nicolike.cn

PHP:  // 无泛型
来源：http://kc.yuexingan06.cn

JS:   // 无泛型
来源：http://gb.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ey.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nt.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oc.gzmigu.cn

Ruby: # 无泛型
来源：http://bs.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wh.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://gx.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tu.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://qh.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://is.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jw.gzmigu.cn

Java: // 无解构
来源：http://mc.hnjuh.cn

Go:   // 无解构
来源：http://qe.panjiajie.cn

Ruby: a, b = pair
来源：http://fh.colortex.cn

C#:   var (a, b) = pair;
来源：http://hm.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://nf.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iz.jctech888.com.cn

PHP:  // 无重载
来源：http://dg.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rs.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://np.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vr.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://ik.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://qj.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qq.9csxet.cn

================================================================================
来源：http://dq.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://yo.wgjwhj.cn

================================================================================
来源：http://zz.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://eg.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lj.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rf.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://va.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ck.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ba.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zr.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://kj.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nc.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://lf.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ga.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xk.muxihuayi.cn

JS:   arr.push(4);
来源：http://wj.bookmarksfly.cn

TS:   arr.push(4);
来源：http://gi.muxihuayi.cn

Java: list.add(4);
来源：http://xq.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ya.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jd.haigaiapp.cn

C#:   list.Add(4);
来源：http://ug.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://vw.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://bj.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://be.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iv.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://um.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://ra.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pz.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://bp.yuexingan06.cn

[D04] 删除元素
来源：http://hd.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fu.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://il.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rv.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://hh.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ja.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://am.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uu.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ht.hahajie.cn

[D05] 访问与修改元素
来源：http://tr.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hr.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pv.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pf.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://jt.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://yi.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://xw.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yp.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zf.asd995.cn

[D06] 数组长度
来源：http://ab.hahajie.cn

Py:   len(arr)
来源：http://fy.shxzskj.cn

PHP:  count($arr);
来源：http://ce.shxzskj.cn

JS:   arr.length
来源：http://rn.lnxyls.cn

TS:   arr.length
来源：http://qp.wgjwhj.cn

Java: list.size();
来源：http://mw.asd995.cn

Go:   len(arr)
来源：http://yi.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://hu.szxytkj.cn

C#:   list.Count;
来源：http://mb.hahajie.cn

[D07] 切片 / 取子数组
来源：http://nl.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lq.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://og.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://pj.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://yj.szxytkj.cn

Java: list.subList(1, 4);
来源：http://nm.shtwfgs.cn

Go:   arr[1:4]
来源：http://vt.shxzukj.cn

Ruby: arr[1, 3]
来源：http://rx.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://hz.nszjky.cn

[D08] 合并两个数组
来源：http://kq.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://em.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ru.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pv.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://rz.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gy.521024.cn

Go:   append(a, b...)
来源：http://vp.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://xp.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://ui.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://uo.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ro.huixiangedu.cn

PHP:  sort($arr);
来源：http://mz.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ha.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tj.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oh.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ff.colortex.cn

Ruby: arr.sort
来源：http://qn.9csxet.cn

C#:   list.Sort();
来源：http://ht.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qy.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yv.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wg.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fc.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oy.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xb.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ak.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yw.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mj.shxzskj.cn

[D11] 反转数组
来源：http://vp.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vt.hahajie.cn

PHP:  array_reverse($arr);
来源：http://so.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pd.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://kx.newstarts.cn

Java: Collections.reverse(list);
来源：http://at.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://up.hnjuh.cn

Ruby: arr.reverse
来源：http://lu.lnxyls.cn

C#:   list.Reverse();
来源：http://xk.521024.cn

[D12] 查找元素下标
来源：http://dr.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://vu.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://an.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ok.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qx.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xq.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://gf.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ng.szsharing.cn

C#:   list.IndexOf(x);
来源：http://by.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://yr.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xq.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qs.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://ws.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://xo.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bi.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://po.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lk.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bj.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://gu.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hc.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://js.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://ey.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://qw.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cr.9csxet.cn

Go:   // 手写循环
来源：http://wz.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dc.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yz.yuexingan06.cn

[D15] 去重
来源：http://jb.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qp.huanxung.cn

PHP:  array_unique($arr);
来源：http://fq.nszjky.cn

JS:   [...new Set(arr)]
来源：http://qj.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://zs.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gj.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wu.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://su.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ks.hahajie.cn

[D16] 求和与平均值
来源：http://rt.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sz.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gh.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uc.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ug.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dt.huixiangedu.cn

Go:   // 手写循环累加
来源：http://pn.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ts.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://ly.huanxung.cn

[D17] 最大值与最小值
来源：http://tr.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://cw.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://ln.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xz.gzmigu.cn

TS:   Math.max(...arr);
来源：http://vv.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ac.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yh.colortex.cn

Ruby: arr.max;  arr.min
来源：http://cf.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://ea.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://yh.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ap.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://et.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tc.hnjuh.cn

TS:   nested.flat();
来源：http://gn.hahajie.cn


<!-- 参考信息 -->