代发 wailian999

Py:   if not data: return
来源：http://sk.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://bn.bjjhwx.cn

JS:   if (!data) return;
来源：http://co.muxihuayi.cn

TS:   if (!data) return;
来源：http://uy.panjiajie.cn

Java: if (data == null) return;
来源：http://lt.hahajie.cn

Go:   if data == nil { return }
来源：http://qv.shtwfgs.cn

Ruby: return if data.nil?
来源：http://as.521024.cn

C#:   if (data == null) return;
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://vp.bjjhwx.cn

C. 函数与作用域
来源：http://iw.jctech888.com.cn

================================================================================
来源：http://ta.hahajie.cn

[C01] 定义函数
来源：http://xl.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://og.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uy.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://mr.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gi.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gr.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tg.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://vh.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ef.szsharing.cn

[C02] 默认参数
来源：http://vg.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://wm.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uk.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://nx.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hu.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oa.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lf.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://ob.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://jd.nszjky.cn

[C03] 可变参数
来源：http://lm.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://pg.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sx.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://po.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oc.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://os.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pl.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kz.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://us.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sx.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nl.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fi.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kr.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://yv.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://tm.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://aa.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://cz.wgjwhj.cn

[C05] 返回多个值
来源：http://mv.yuexingan06.cn

Py:   return a, b
来源：http://go.shxzskj.cn

PHP:  return [$a, $b];
来源：http://kt.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bd.hnjuh.cn

TS:   return { a, b };
来源：http://xr.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fj.nicolike.cn

Go:   return a, b
来源：http://ht.asd995.cn

Ruby: return a, b
来源：http://nc.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://sp.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://qd.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://zz.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qn.panjiajie.cn

JS:   const square = x => x * x;
来源：http://nt.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ai.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cc.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wr.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://ci.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://du.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://rq.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yf.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tm.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fk.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://ge.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nn.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cm.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ys.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yi.lnxyls.cn

[C08] 闭包
来源：http://ov.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ls.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dc.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cl.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://av.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nq.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://af.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ls.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gz.bookmarksfly.cn

[C09] 递归
来源：http://zi.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://he.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uh.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jm.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fd.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lx.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eb.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ai.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wb.jctech888.com.cn

[C10] 变量作用域
来源：http://il.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://al.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fe.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gf.lnxyls.cn

TS:   同 JS
来源：http://xs.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://nh.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://vr.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rq.bjjhwx.cn

C#:   块级作用域
来源：http://iu.newstarts.cn

[C11] 模块导入与导出
来源：http://dd.panjiajie.cn

Py:   from module import func
来源：http://hd.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sd.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gu.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yz.lnxyls.cn

Java: import java.util.List;
来源：http://er.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ug.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://zw.bjjhwx.cn

C#:   using System.Text;
来源：http://dt.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://te.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://gl.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ko.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://qm.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://gu.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xj.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://tq.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://be.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bv.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://fn.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vu.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xc.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tu.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hl.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dh.9csxet.cn

Go:   func add(a, b int) int
来源：http://zc.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://up.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://li.huixiangedu.cn

[C14] 泛型函数
来源：http://dx.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sp.bookmarksfly.cn

PHP:  // 无泛型
来源：http://cq.yuexingan06.cn

JS:   // 无泛型
来源：http://pg.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ul.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://au.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zi.jctech888.com.cn

Ruby: # 无泛型
来源：http://cv.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mw.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://yd.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ox.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://fj.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dw.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fx.hahajie.cn

Java: // 无解构
来源：http://gz.hnjuh.cn

Go:   // 无解构
来源：http://bd.gzmigu.cn

Ruby: a, b = pair
来源：http://ft.521024.cn

C#:   var (a, b) = pair;
来源：http://en.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://kp.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://am.bjjhwx.cn

PHP:  // 无重载
来源：http://vy.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fa.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://zb.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jx.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ro.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ir.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vr.hahajie.cn

================================================================================
来源：http://rq.521024.cn

D. 数组 / 列表 / 集合
来源：http://dz.9csxet.cn

================================================================================
来源：http://as.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://fs.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bu.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gt.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cj.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hy.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tc.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zn.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://jl.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://la.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://ho.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fk.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tf.shtwfgs.cn

JS:   arr.push(4);
来源：http://bk.bjjhwx.cn

TS:   arr.push(4);
来源：http://xq.huanxung.cn

Java: list.add(4);
来源：http://he.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://mh.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://hr.hnjuh.cn

C#:   list.Add(4);
来源：http://yl.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://hx.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://dc.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gc.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bc.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://bk.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://ng.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fg.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xd.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://oe.huixiangedu.cn

[D04] 删除元素
来源：http://yt.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gy.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zk.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jd.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://ye.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rc.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bo.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wl.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ii.colortex.cn

[D05] 访问与修改元素
来源：http://qk.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vu.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xd.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bk.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://up.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://sn.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://nz.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gp.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ef.bookmarksfly.cn

[D06] 数组长度
来源：http://jx.nicolike.cn

Py:   len(arr)
来源：http://cd.asd995.cn

PHP:  count($arr);
来源：http://wz.szxytkj.cn

JS:   arr.length
来源：http://qq.nicolike.cn

TS:   arr.length
来源：http://jp.shxzskj.cn

Java: list.size();
来源：http://kt.hahajie.cn

Go:   len(arr)
来源：http://tb.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://oz.hnjuh.cn

C#:   list.Count;
来源：http://io.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ew.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://db.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qa.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://xt.521024.cn

TS:   arr.slice(1, 4);
来源：http://pa.hahajie.cn

Java: list.subList(1, 4);
来源：http://dg.haigaiapp.cn

Go:   arr[1:4]
来源：http://ki.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://lo.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://md.wgjwhj.cn

[D08] 合并两个数组
来源：http://mh.521024.cn

Py:   a + b;  a.extend(b)
来源：http://cc.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://vl.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://du.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ep.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vr.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ig.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://zd.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://fg.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://xi.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://cp.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://qb.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qh.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lv.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jt.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wt.lnxyls.cn

Ruby: arr.sort
来源：http://sl.shxzukj.cn

C#:   list.Sort();
来源：http://ns.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cz.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vz.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tb.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hi.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://te.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yk.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kj.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xm.bookmarksfly.cn

[D11] 反转数组
来源：http://dp.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yp.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://ey.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uc.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://jo.hahajie.cn

Java: Collections.reverse(list);
来源：http://lf.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://iy.wgjwhj.cn

Ruby: arr.reverse
来源：http://ec.hahajie.cn

C#:   list.Reverse();
来源：http://og.hnjuh.cn

[D12] 查找元素下标
来源：http://oc.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://fs.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xi.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sp.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kr.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ot.521024.cn

Go:   slices.Index(arr, x)
来源：http://nd.asd995.cn

Ruby: arr.index(x)
来源：http://ep.521024.cn

C#:   list.IndexOf(x);
来源：http://ta.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://di.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fm.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zz.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://sk.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://fg.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qj.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nd.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yu.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://da.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://ar.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ls.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kp.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://eg.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://gp.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vb.szxytkj.cn

Go:   // 手写循环
来源：http://ju.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gp.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jv.asd995.cn

[D15] 去重
来源：http://ka.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zm.colortex.cn

PHP:  array_unique($arr);
来源：http://cp.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://bd.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ti.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jy.gzmigu.cn

Ruby: arr.uniq
来源：http://it.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://gt.haigaiapp.cn

[D16] 求和与平均值
来源：http://by.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://di.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fp.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bm.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oo.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ii.lnxyls.cn

Go:   // 手写循环累加
来源：http://wk.bookmarksfly.cn


<!-- 参考信息 -->