代发 wailian999

Go:   a && b || !c
来源：http://rp.jctech888.com.cn

Ruby: a && b || !c
来源：http://uc.haigaiapp.cn

C#:   a && b || !c
来源：http://eh.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yr.gzmigu.cn

Py:   if not data: return
来源：http://bt.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://ap.521024.cn

JS:   if (!data) return;
来源：http://dp.shtwfgs.cn

TS:   if (!data) return;
来源：http://ly.shtwfgs.cn

Java: if (data == null) return;
来源：http://bk.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://tg.hahajie.cn

Ruby: return if data.nil?
来源：http://ov.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://df.haigaiapp.cn

================================================================================
来源：http://vt.huixiangedu.cn

C. 函数与作用域
来源：http://qi.hnjuh.cn

================================================================================
来源：http://dp.huixiangedu.cn

[C01] 定义函数
来源：http://um.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://cr.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wx.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://zh.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lv.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qw.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oy.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://us.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oo.szsharing.cn

[C02] 默认参数
来源：http://gk.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://cj.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ze.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://tz.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nb.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lk.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://na.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://cl.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://av.jianghongdianzi.cn

[C03] 可变参数
来源：http://vg.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://cb.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lu.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://px.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ab.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zl.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hp.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mb.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dx.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xs.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lr.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qv.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://bq.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://hg.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://wb.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://wx.wgjwhj.cn

[C05] 返回多个值
来源：http://ne.asd995.cn

Py:   return a, b
来源：http://ol.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://sc.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xb.9csxet.cn

TS:   return { a, b };
来源：http://de.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wz.bjjhwx.cn

Go:   return a, b
来源：http://lj.wgjwhj.cn

Ruby: return a, b
来源：http://rs.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://is.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://af.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://ln.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zm.521024.cn

JS:   const square = x => x * x;
来源：http://tu.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ni.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://em.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hu.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://xr.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ip.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://er.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ma.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xk.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pd.nszjky.cn

TS:   arr.map(String)
来源：http://fc.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vv.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dm.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://bn.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dx.huanxung.cn

[C08] 闭包
来源：http://bu.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gi.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wy.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vn.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bb.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ja.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xb.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yi.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ag.nicolike.cn

[C09] 递归
来源：http://gx.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cg.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fw.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hs.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sy.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://py.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rn.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sy.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://br.shxzskj.cn

[C10] 变量作用域
来源：http://nm.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nz.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ex.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rt.newstarts.cn

TS:   同 JS
来源：http://fm.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://zk.9csxet.cn

Go:   花括号块级作用域
来源：http://fl.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gp.bjjhwx.cn

C#:   块级作用域
来源：http://wr.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://kl.huanxung.cn

Py:   from module import func
来源：http://wn.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yw.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ur.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zn.huixinmuqiang.cn

Java: import java.util.List;
来源：http://kg.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gk.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://hv.hnjuh.cn

C#:   using System.Text;
来源：http://aw.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://fv.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://dn.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://hw.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://pa.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://qn.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ry.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://wg.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://jm.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://na.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://la.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tf.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pk.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://os.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jk.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://qk.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vh.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dd.gzmigu.cn

[C14] 泛型函数
来源：http://tv.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ed.9csxet.cn

PHP:  // 无泛型
来源：http://mc.nicolike.cn

JS:   // 无泛型
来源：http://ih.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wg.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xz.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://up.wgjwhj.cn

Ruby: # 无泛型
来源：http://kl.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yl.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://sb.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yt.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://pb.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xg.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ua.colortex.cn

Java: // 无解构
来源：http://eq.nicolike.cn

Go:   // 无解构
来源：http://ox.muxihuayi.cn

Ruby: a, b = pair
来源：http://ab.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://qa.colortex.cn

[C16] 函数 / 方法重载
来源：http://ps.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xf.wgjwhj.cn

PHP:  // 无重载
来源：http://sc.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rc.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://je.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ew.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://uy.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ry.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ba.521024.cn

================================================================================
来源：http://mx.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://vr.shxzukj.cn

================================================================================
来源：http://my.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://pr.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oz.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kc.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fq.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jk.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qd.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://hb.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ov.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nb.nicolike.cn

[D02] 追加元素到末尾
来源：http://od.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oo.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jp.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://dx.panjiajie.cn

TS:   arr.push(4);
来源：http://zi.jctech888.com.cn

Java: list.add(4);
来源：http://jq.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://gp.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://gy.asd995.cn

C#:   list.Add(4);
来源：http://px.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://uc.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://km.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://os.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ar.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://kg.huanxung.cn

Java: list.add(0, 0);
来源：http://cu.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zh.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wd.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://js.panjiajie.cn

[D04] 删除元素
来源：http://xb.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ga.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yv.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hm.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://op.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ex.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://er.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gn.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ge.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ul.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vm.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ec.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ql.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://tc.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://sr.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://de.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://am.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mq.bjjhwx.cn

[D06] 数组长度
来源：http://it.bookmarksfly.cn

Py:   len(arr)
来源：http://eq.yuexingan06.cn

PHP:  count($arr);
来源：http://dm.asd995.cn

JS:   arr.length
来源：http://ty.shtwfgs.cn

TS:   arr.length
来源：http://gz.jianghongdianzi.cn

Java: list.size();
来源：http://vr.shtwfgs.cn

Go:   len(arr)
来源：http://ma.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://og.jctech888.com.cn

C#:   list.Count;
来源：http://pg.asd995.cn

[D07] 切片 / 取子数组
来源：http://fi.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://la.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oz.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://lr.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://qq.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ej.chemitech.net.cn

Go:   arr[1:4]
来源：http://rt.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://as.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://nb.huanxung.cn

[D08] 合并两个数组
来源：http://cv.521024.cn

Py:   a + b;  a.extend(b)
来源：http://vm.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://ge.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://io.wgjwhj.cn

TS:   [...a, ...b];
来源：http://dl.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pj.nicolike.cn

Go:   append(a, b...)
来源：http://oj.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://lb.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://yf.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://tt.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://rz.haigaiapp.cn

PHP:  sort($arr);
来源：http://xa.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pl.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wp.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://br.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pd.gzmigu.cn

Ruby: arr.sort
来源：http://lo.szsharing.cn

C#:   list.Sort();
来源：http://xg.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jv.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://na.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kf.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zx.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vj.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ss.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dd.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jd.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nv.hahajie.cn

[D11] 反转数组
来源：http://su.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eh.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://ye.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://it.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://in.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://sd.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://rm.bookmarksfly.cn

Ruby: arr.reverse
来源：http://vy.521024.cn

C#:   list.Reverse();
来源：http://ax.asd995.cn

[D12] 查找元素下标
来源：http://ue.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://yp.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fo.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oo.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gg.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rr.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://lf.shtwfgs.cn

Ruby: arr.index(x)
来源：http://vp.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ee.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://kt.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vr.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cv.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://ba.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://nf.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rt.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ec.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pm.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://on.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://wp.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uy.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pd.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://ge.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://yh.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oq.yuntaijiaju.cn

Go:   // 手写循环
来源：http://wn.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ld.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yl.szsharing.cn

[D15] 去重
来源：http://el.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mf.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://kz.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://dj.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://ng.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://td.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ma.lnxyls.cn

Ruby: arr.uniq
来源：http://ei.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://az.muxihuayi.cn

[D16] 求和与平均值
来源：http://zm.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mk.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sg.hahajie.cn


<!-- 参考信息 -->