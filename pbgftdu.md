代发 wailian999

C#:   x is int or double or decimal
来源：http://bn.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://ho.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jt.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wb.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://nk.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://oy.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://la.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pz.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://up.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kw.szxytkj.cn

[B15] 布尔运算与取反
来源：http://jx.huixiangedu.cn

Py:   a and b or not c
来源：http://os.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ib.panjiajie.cn

JS:   a && b || !c
来源：http://le.huixiangedu.cn

TS:   a && b || !c
来源：http://jq.huanxung.cn

Java: a && b || !c
来源：http://ld.jctech888.com.cn

Go:   a && b || !c
来源：http://bh.haigaiapp.cn

Ruby: a && b || !c
来源：http://qj.colortex.cn

C#:   a && b || !c
来源：http://hm.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hr.shtwfgs.cn

Py:   if not data: return
来源：http://hg.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://gd.shtwfgs.cn

JS:   if (!data) return;
来源：http://vf.yuexingan06.cn

TS:   if (!data) return;
来源：http://dx.lnxyls.cn

Java: if (data == null) return;
来源：http://qq.muxihuayi.cn

Go:   if data == nil { return }
来源：http://fs.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://hh.wgjwhj.cn

C#:   if (data == null) return;
来源：http://rc.chemitech.net.cn

================================================================================
来源：http://zp.colortex.cn

C. 函数与作用域
来源：http://ry.huixinmuqiang.cn

================================================================================
来源：http://ez.shxzskj.cn

[C01] 定义函数
来源：http://yh.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://lj.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jg.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://jj.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dd.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ic.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fs.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ks.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eg.shxzskj.cn

[C02] 默认参数
来源：http://gf.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://tz.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ep.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://qq.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jw.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wl.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lh.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://db.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://cq.newstarts.cn

[C03] 可变参数
来源：http://nv.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://fl.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ru.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kg.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cx.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ik.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pa.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pj.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yl.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://md.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wq.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nh.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dh.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://kd.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://zk.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://wn.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://es.hnjuh.cn

[C05] 返回多个值
来源：http://ul.shtwfgs.cn

Py:   return a, b
来源：http://ga.colortex.cn

PHP:  return [$a, $b];
来源：http://iq.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sx.muxihuayi.cn

TS:   return { a, b };
来源：http://za.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ba.asd995.cn

Go:   return a, b
来源：http://pj.gzmigu.cn

Ruby: return a, b
来源：http://ct.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ft.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://ik.nszjky.cn

Py:   square = lambda x: x * x
来源：http://co.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zd.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ju.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://mf.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sa.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tu.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://hb.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vv.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://lo.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ds.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iw.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rn.asd995.cn

TS:   arr.map(String)
来源：http://xa.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ye.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dt.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://sb.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hv.huanxung.cn

[C08] 闭包
来源：http://fd.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mr.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yo.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ct.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uu.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kk.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jg.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lv.szxytkj.cn

[C09] 递归
来源：http://wb.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ky.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cp.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wb.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ca.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gn.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kq.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rw.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vf.chemitech.net.cn

[C10] 变量作用域
来源：http://ij.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ox.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ee.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ny.szsharing.cn

TS:   同 JS
来源：http://fz.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ow.colortex.cn

Go:   花括号块级作用域
来源：http://wl.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kn.chemitech.net.cn

C#:   块级作用域
来源：http://kp.newstarts.cn

[C11] 模块导入与导出
来源：http://iu.9csxet.cn

Py:   from module import func
来源：http://hz.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dv.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://di.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kw.wgjwhj.cn

Java: import java.util.List;
来源：http://ux.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sk.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://pk.lnxyls.cn

C#:   using System.Text;
来源：http://wk.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://af.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://yu.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://uf.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://zr.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://el.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zo.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://zg.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://zn.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ba.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://hj.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kf.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lc.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cy.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ky.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pi.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://ly.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pf.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wx.nszjky.cn

[C14] 泛型函数
来源：http://wk.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ho.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://oz.asd995.cn

JS:   // 无泛型
来源：http://qn.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jv.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mo.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jc.9csxet.cn

Ruby: # 无泛型
来源：http://rd.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rt.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://le.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qo.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ah.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ex.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oi.shxzskj.cn

Java: // 无解构
来源：http://vd.shtwfgs.cn

Go:   // 无解构
来源：http://yh.shxzskj.cn

Ruby: a, b = pair
来源：http://ji.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://jv.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://rm.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qt.gzmigu.cn

PHP:  // 无重载
来源：http://ja.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ry.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://do.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ph.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://rr.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://at.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fj.nszjky.cn

================================================================================
来源：http://ui.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://um.bjjhwx.cn

================================================================================
来源：http://jh.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://dq.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://em.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ug.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://su.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wm.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kx.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://nb.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://tg.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bc.colortex.cn

[D02] 追加元素到末尾
来源：http://eo.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nc.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ri.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ge.szsharing.cn

TS:   arr.push(4);
来源：http://jp.gzmigu.cn

Java: list.add(4);
来源：http://me.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://hx.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://po.huixiangedu.cn

C#:   list.Add(4);
来源：http://cw.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ws.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://dj.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bu.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ur.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://af.9csxet.cn

Java: list.add(0, 0);
来源：http://yy.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vf.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bm.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ec.wgjwhj.cn

[D04] 删除元素
来源：http://yd.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xr.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ts.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vk.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://nn.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zy.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hj.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://te.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://re.haigaiapp.cn

[D05] 访问与修改元素
来源：http://cs.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sd.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yr.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ov.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ud.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://pj.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://pz.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oc.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ts.newstarts.cn

[D06] 数组长度
来源：http://pl.haigaiapp.cn

Py:   len(arr)
来源：http://hj.asd995.cn

PHP:  count($arr);
来源：http://zd.panjiajie.cn

JS:   arr.length
来源：http://ru.haigaiapp.cn

TS:   arr.length
来源：http://qb.shtwfgs.cn

Java: list.size();
来源：http://ww.haigaiapp.cn

Go:   len(arr)
来源：http://fy.521024.cn

Ruby: arr.length; arr.size
来源：http://zy.haigaiapp.cn

C#:   list.Count;
来源：http://cu.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://nj.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fe.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gl.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://hx.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ms.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://gg.521024.cn

Go:   arr[1:4]
来源：http://zr.hnjuh.cn

Ruby: arr[1, 3]
来源：http://of.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://he.wgjwhj.cn

[D08] 合并两个数组
来源：http://ha.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://tk.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://pq.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qx.hahajie.cn

TS:   [...a, ...b];
来源：http://zz.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sf.yuexingan06.cn

Go:   append(a, b...)
来源：http://xb.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://wz.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://dc.asd995.cn

[D09] 排序（升序）
来源：http://yh.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ss.nszjky.cn

PHP:  sort($arr);
来源：http://gx.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://st.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ci.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nk.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fu.muxihuayi.cn

Ruby: arr.sort
来源：http://cv.hahajie.cn

C#:   list.Sort();
来源：http://cc.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ih.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pc.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mb.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yt.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qg.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yf.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xm.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mc.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hk.wgjwhj.cn

[D11] 反转数组
来源：http://lc.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://au.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://ct.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vi.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://dq.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://yd.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ei.shtwfgs.cn

Ruby: arr.reverse
来源：http://uq.nicolike.cn

C#:   list.Reverse();
来源：http://mv.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://bd.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://xd.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bh.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nu.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kw.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rc.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://oq.panjiajie.cn

Ruby: arr.index(x)
来源：http://rh.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://xv.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://hr.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zi.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wp.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://ss.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://du.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ao.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://br.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dk.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fy.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://es.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ob.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hc.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://lw.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://gf.shtwfgs.cn


<!-- 参考信息 -->