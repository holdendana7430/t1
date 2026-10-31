代发 wailian999

C#:   x is int or double or decimal
来源：http://qi.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://fn.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fi.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qq.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://qz.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://ij.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://it.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xe.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ys.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xu.gzmigu.cn

[B15] 布尔运算与取反
来源：http://sr.jctech888.com.cn

Py:   a and b or not c
来源：http://ja.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://uz.panjiajie.cn

JS:   a && b || !c
来源：http://fw.shxzukj.cn

TS:   a && b || !c
来源：http://pi.wgjwhj.cn

Java: a && b || !c
来源：http://rd.asd995.cn

Go:   a && b || !c
来源：http://bw.szxytkj.cn

Ruby: a && b || !c
来源：http://wi.chemitech.net.cn

C#:   a && b || !c
来源：http://km.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://id.lnxyls.cn

Py:   if not data: return
来源：http://hr.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://xn.panjiajie.cn

JS:   if (!data) return;
来源：http://mw.jctech888.com.cn

TS:   if (!data) return;
来源：http://rw.lnxyls.cn

Java: if (data == null) return;
来源：http://nc.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://iy.chemitech.net.cn

Ruby: return if data.nil?
来源：http://hd.nszjky.cn

C#:   if (data == null) return;
来源：http://tr.9csxet.cn

================================================================================
来源：http://gb.huanxung.cn

C. 函数与作用域
来源：http://dt.shxzskj.cn

================================================================================
来源：http://yb.yuntaijiaju.cn

[C01] 定义函数
来源：http://pa.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://bq.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yd.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://wo.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iq.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ue.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qm.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://th.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ix.bookmarksfly.cn

[C02] 默认参数
来源：http://zq.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://fl.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iu.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://hc.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fn.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bs.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ww.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://xw.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ar.huanxung.cn

[C03] 可变参数
来源：http://br.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://rz.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dm.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jj.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yc.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tj.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mu.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xp.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yj.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://qz.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cu.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sv.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nr.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://di.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://fr.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://el.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://sx.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://ej.jctech888.com.cn

[C05] 返回多个值
来源：http://bv.haigaiapp.cn

Py:   return a, b
来源：http://lu.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://nw.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bt.colortex.cn

TS:   return { a, b };
来源：http://qg.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cg.hnjuh.cn

Go:   return a, b
来源：http://bd.panjiajie.cn

Ruby: return a, b
来源：http://gi.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://up.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://kp.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://vh.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dm.huanxung.cn

JS:   const square = x => x * x;
来源：http://yk.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://hs.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gj.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fq.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://er.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vr.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://im.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lp.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eb.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://on.colortex.cn

TS:   arr.map(String)
来源：http://tf.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ig.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cg.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://ro.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cv.newstarts.cn

[C08] 闭包
来源：http://uq.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ey.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vk.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kq.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wx.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ml.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lc.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pi.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rr.nszjky.cn

[C09] 递归
来源：http://tu.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gn.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://po.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tx.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ko.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vg.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://am.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dg.shxzskj.cn

[C10] 变量作用域
来源：http://ca.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wt.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fa.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nr.bjjhwx.cn

TS:   同 JS
来源：http://hu.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://jg.huixiangedu.cn

Go:   花括号块级作用域
来源：http://fy.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tm.asd995.cn

C#:   块级作用域
来源：http://pp.panjiajie.cn

[C11] 模块导入与导出
来源：http://aw.haigaiapp.cn

Py:   from module import func
来源：http://or.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ua.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ql.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yn.newstarts.cn

Java: import java.util.List;
来源：http://pb.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ok.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://yz.muxihuayi.cn

C#:   using System.Text;
来源：http://cu.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://iy.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://jo.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://fk.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://xw.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://pv.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sy.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://jo.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://zu.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ww.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://mc.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cb.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fc.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://me.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rn.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fh.nszjky.cn

Go:   func add(a, b int) int
来源：http://fd.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rr.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wx.szxytkj.cn

[C14] 泛型函数
来源：http://df.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rf.gzmigu.cn

PHP:  // 无泛型
来源：http://gk.nicolike.cn

JS:   // 无泛型
来源：http://od.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ee.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qt.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cw.newstarts.cn

Ruby: # 无泛型
来源：http://iz.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://id.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://ro.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lz.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://up.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ky.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ob.huixiangedu.cn

Java: // 无解构
来源：http://mb.nszjky.cn

Go:   // 无解构
来源：http://va.521024.cn

Ruby: a, b = pair
来源：http://bd.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://pm.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://oh.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hn.yuntaijiaju.cn

PHP:  // 无重载
来源：http://ux.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://se.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ti.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zw.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://wd.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://cr.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tr.hahajie.cn

================================================================================
来源：http://ll.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://gg.shxzukj.cn

================================================================================
来源：http://je.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://wi.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fa.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sa.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zr.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gp.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dh.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://ih.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://sp.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.nszjky.cn

[D02] 追加元素到末尾
来源：http://rn.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mm.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yz.shtwfgs.cn

JS:   arr.push(4);
来源：http://jm.asd995.cn

TS:   arr.push(4);
来源：http://ad.jianghongdianzi.cn

Java: list.add(4);
来源：http://tw.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://as.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://zy.hnjuh.cn

C#:   list.Add(4);
来源：http://dw.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://kk.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://bo.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://na.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tb.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://ag.9csxet.cn

Java: list.add(0, 0);
来源：http://ek.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nf.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pr.asd995.cn

C#:   list.Insert(0, 0);
来源：http://aw.shxzskj.cn

[D04] 删除元素
来源：http://hs.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pz.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nx.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fa.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://tn.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fg.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hu.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pa.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dh.colortex.cn

[D05] 访问与修改元素
来源：http://bm.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://va.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aj.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xb.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://nb.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://pw.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://lj.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hx.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rs.hahajie.cn

[D06] 数组长度
来源：http://yp.newstarts.cn

Py:   len(arr)
来源：http://we.gzmigu.cn

PHP:  count($arr);
来源：http://fk.9csxet.cn

JS:   arr.length
来源：http://sq.jctech888.com.cn

TS:   arr.length
来源：http://sb.bookmarksfly.cn

Java: list.size();
来源：http://cs.huixinmuqiang.cn

Go:   len(arr)
来源：http://ad.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://vr.nszjky.cn

C#:   list.Count;
来源：http://ez.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://kj.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eg.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mm.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://ay.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://et.nszjky.cn

Java: list.subList(1, 4);
来源：http://fw.chemitech.net.cn

Go:   arr[1:4]
来源：http://tc.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://tb.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://vq.szxytkj.cn

[D08] 合并两个数组
来源：http://am.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://od.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://ti.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nw.newstarts.cn

TS:   [...a, ...b];
来源：http://vy.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fm.shtwfgs.cn

Go:   append(a, b...)
来源：http://vn.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://jz.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://na.lnxyls.cn

[D09] 排序（升序）
来源：http://oy.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://hy.szsharing.cn

PHP:  sort($arr);
来源：http://vo.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zs.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zi.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cl.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lx.huixinmuqiang.cn

Ruby: arr.sort
来源：http://wr.521024.cn

C#:   list.Sort();
来源：http://ni.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ni.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yj.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nl.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://by.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ea.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ea.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wm.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ic.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xx.szxytkj.cn

[D11] 反转数组
来源：http://bb.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oy.huanxung.cn

PHP:  array_reverse($arr);
来源：http://wi.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zk.szxytkj.cn

TS:   [...arr].reverse();
来源：http://fs.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://tc.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://yq.521024.cn

Ruby: arr.reverse
来源：http://bb.shtwfgs.cn

C#:   list.Reverse();
来源：http://qp.9csxet.cn

[D12] 查找元素下标
来源：http://oz.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://ki.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bp.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gp.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yb.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://et.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://lh.huanxung.cn

Ruby: arr.index(x)
来源：http://yx.521024.cn

C#:   list.IndexOf(x);
来源：http://cr.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://om.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vh.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tr.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://tn.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://xe.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fl.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mp.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fn.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fn.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://dh.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dl.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oj.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://jf.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://jb.9csxet.cn


<!-- 参考信息 -->