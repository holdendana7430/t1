代发 wailian999

Go:   a && b || !c
来源：http://gj.jctech888.com.cn

Ruby: a && b || !c
来源：http://dx.szsharing.cn

C#:   a && b || !c
来源：http://ng.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ma.panjiajie.cn

Py:   if not data: return
来源：http://jp.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://ef.colortex.cn

JS:   if (!data) return;
来源：http://rd.nicolike.cn

TS:   if (!data) return;
来源：http://lg.shxzskj.cn

Java: if (data == null) return;
来源：http://kq.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ie.chemitech.net.cn

Ruby: return if data.nil?
来源：http://tz.shxzskj.cn

C#:   if (data == null) return;
来源：http://wg.hahajie.cn

================================================================================
来源：http://fl.yuexingan06.cn

C. 函数与作用域
来源：http://xz.hnjuh.cn

================================================================================
来源：http://pq.panjiajie.cn

[C01] 定义函数
来源：http://wi.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://gv.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ng.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://rw.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://up.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://re.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lx.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://ov.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://du.colortex.cn

[C02] 默认参数
来源：http://nk.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://qf.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dd.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tt.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lk.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jd.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bz.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://vp.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ui.wgjwhj.cn

[C03] 可变参数
来源：http://cv.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://lu.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pr.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://if.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vv.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hp.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://op.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ru.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ih.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lx.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tf.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ca.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oz.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://sf.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ys.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ab.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://yf.521024.cn

[C05] 返回多个值
来源：http://ry.szxytkj.cn

Py:   return a, b
来源：http://df.521024.cn

PHP:  return [$a, $b];
来源：http://mo.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fi.muxihuayi.cn

TS:   return { a, b };
来源：http://kh.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://od.yuexingan06.cn

Go:   return a, b
来源：http://mm.newstarts.cn

Ruby: return a, b
来源：http://mi.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://uy.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ji.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://id.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ws.nicolike.cn

JS:   const square = x => x * x;
来源：http://aa.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://au.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qk.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hd.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://xu.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gr.nicolike.cn

[C07] 把函数作为参数传入
来源：http://uq.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://br.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ud.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cd.bjjhwx.cn

TS:   arr.map(String)
来源：http://jd.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bb.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nt.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://na.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qd.szxytkj.cn

[C08] 闭包
来源：http://kd.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dv.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sj.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wr.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qb.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nj.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pq.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yx.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://we.wgjwhj.cn

[C09] 递归
来源：http://ln.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xc.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tq.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vq.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dc.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dh.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pb.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://my.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xb.shxzskj.cn

[C10] 变量作用域
来源：http://ff.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ia.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xu.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ve.huixinmuqiang.cn

TS:   同 JS
来源：http://ob.9csxet.cn

Java: 方法内为块级作用域
来源：http://wo.bjjhwx.cn

Go:   花括号块级作用域
来源：http://pg.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rt.bjjhwx.cn

C#:   块级作用域
来源：http://ad.newstarts.cn

[C11] 模块导入与导出
来源：http://yz.muxihuayi.cn

Py:   from module import func
来源：http://en.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mq.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://on.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dj.shtwfgs.cn

Java: import java.util.List;
来源：http://ck.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dx.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://sp.szxytkj.cn

C#:   using System.Text;
来源：http://yf.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ld.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://wm.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://sv.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://pp.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ix.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kq.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://wp.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://ap.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gl.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://qn.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qr.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sc.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sx.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ci.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://te.colortex.cn

Go:   func add(a, b int) int
来源：http://wg.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tc.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qq.yuexingan06.cn

[C14] 泛型函数
来源：http://mf.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://be.gzmigu.cn

PHP:  // 无泛型
来源：http://aa.huixiangedu.cn

JS:   // 无泛型
来源：http://yz.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hg.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ay.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uh.hahajie.cn

Ruby: # 无泛型
来源：http://kz.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bs.szsharing.cn

[C15] 解构 / 展开参数
来源：http://wl.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cr.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://wa.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uq.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ig.jianghongdianzi.cn

Java: // 无解构
来源：http://re.newstarts.cn

Go:   // 无解构
来源：http://cp.bookmarksfly.cn

Ruby: a, b = pair
来源：http://xy.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://wi.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://wu.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://is.bookmarksfly.cn

PHP:  // 无重载
来源：http://zh.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://co.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://oq.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ng.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://nr.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://xj.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vu.hnjuh.cn

================================================================================
来源：http://uq.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://xd.hnjuh.cn

================================================================================
来源：http://dn.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ov.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zb.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fi.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://js.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kq.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fm.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://yz.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://uj.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://px.huanxung.cn

[D02] 追加元素到末尾
来源：http://hi.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pu.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yz.jctech888.com.cn

JS:   arr.push(4);
来源：http://jl.asd995.cn

TS:   arr.push(4);
来源：http://tr.asd995.cn

Java: list.add(4);
来源：http://sv.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://xh.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://mq.huixiangedu.cn

C#:   list.Add(4);
来源：http://nw.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ds.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://hv.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pi.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lr.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://hp.muxihuayi.cn

Java: list.add(0, 0);
来源：http://wp.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ov.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://am.asd995.cn

C#:   list.Insert(0, 0);
来源：http://wv.shtwfgs.cn

[D04] 删除元素
来源：http://ul.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gw.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hq.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xn.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://qz.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://za.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ru.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xu.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vy.lnxyls.cn

[D05] 访问与修改元素
来源：http://kx.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mv.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aa.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://em.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://sq.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://hs.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://xd.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xq.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kz.lnxyls.cn

[D06] 数组长度
来源：http://wr.hnjuh.cn

Py:   len(arr)
来源：http://pl.jianghongdianzi.cn

PHP:  count($arr);
来源：http://fy.wgjwhj.cn

JS:   arr.length
来源：http://yg.yuntaijiaju.cn

TS:   arr.length
来源：http://dw.huixinmuqiang.cn

Java: list.size();
来源：http://oe.muxihuayi.cn

Go:   len(arr)
来源：http://ai.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://tv.asd995.cn

C#:   list.Count;
来源：http://ll.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://rk.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vw.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dy.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://bs.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://rl.asd995.cn

Java: list.subList(1, 4);
来源：http://zf.shtwfgs.cn

Go:   arr[1:4]
来源：http://mw.lnxyls.cn

Ruby: arr[1, 3]
来源：http://rz.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ws.nszjky.cn

[D08] 合并两个数组
来源：http://wd.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://si.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://bm.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://me.shxzskj.cn

TS:   [...a, ...b];
来源：http://dt.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lu.9csxet.cn

Go:   append(a, b...)
来源：http://sl.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://er.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://ml.hahajie.cn

[D09] 排序（升序）
来源：http://fy.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ay.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://uk.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cp.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://du.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ok.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lh.nicolike.cn

Ruby: arr.sort
来源：http://ml.9csxet.cn

C#:   list.Sort();
来源：http://vo.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dk.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oc.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fe.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mk.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vv.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yl.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ko.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jo.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://le.hahajie.cn

[D11] 反转数组
来源：http://vx.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ps.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://wy.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ps.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://ip.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://rg.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://dg.gzmigu.cn

Ruby: arr.reverse
来源：http://ts.haigaiapp.cn

C#:   list.Reverse();
来源：http://uw.nszjky.cn

[D12] 查找元素下标
来源：http://ny.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://nh.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ur.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zs.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wl.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cn.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://gj.yuexingan06.cn

Ruby: arr.index(x)
来源：http://cj.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://xn.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ip.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gl.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://if.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://wh.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://vi.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mc.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wg.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lj.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wn.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://rw.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qg.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pj.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://if.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://sz.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://od.huixinmuqiang.cn

Go:   // 手写循环
来源：http://xr.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lw.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nz.jianghongdianzi.cn

[D15] 去重
来源：http://rd.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tc.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://sx.asd995.cn

JS:   [...new Set(arr)]
来源：http://gx.nszjky.cn

TS:   [...new Set(arr)]
来源：http://mo.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bq.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ju.hnjuh.cn

Ruby: arr.uniq
来源：http://np.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://eh.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://vb.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vv.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xo.panjiajie.cn


<!-- 参考信息 -->