代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://cz.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fi.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qv.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://sp.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://cb.szsharing.cn

[C03] 可变参数
来源：http://dx.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://wy.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bz.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zj.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jz.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cj.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ts.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tn.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qv.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://gz.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://br.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mr.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mi.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zs.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ve.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://bz.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://za.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://aq.hahajie.cn

[C05] 返回多个值
来源：http://gl.gzmigu.cn

Py:   return a, b
来源：http://lx.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://qx.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ev.panjiajie.cn

TS:   return { a, b };
来源：http://pe.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xg.szsharing.cn

Go:   return a, b
来源：http://dg.shxzukj.cn

Ruby: return a, b
来源：http://bz.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://rn.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://sz.521024.cn

Py:   square = lambda x: x * x
来源：http://iw.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qg.szsharing.cn

JS:   const square = x => x * x;
来源：http://tk.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://mx.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kq.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fc.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://gi.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gp.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://bx.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ct.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vy.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://og.chemitech.net.cn

TS:   arr.map(String)
来源：http://lv.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nz.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vw.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://nk.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jd.szxytkj.cn

[C08] 闭包
来源：http://xs.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ca.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ey.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hs.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ia.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oa.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ov.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wm.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hb.jianghongdianzi.cn

[C09] 递归
来源：http://ge.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xj.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rg.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dk.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ad.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vn.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tv.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ou.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gl.hahajie.cn

[C10] 变量作用域
来源：http://hm.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cs.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lf.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nf.521024.cn

TS:   同 JS
来源：http://ui.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ay.szxytkj.cn

Go:   花括号块级作用域
来源：http://vo.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wv.nicolike.cn

C#:   块级作用域
来源：http://oj.colortex.cn

[C11] 模块导入与导出
来源：http://cu.yuexingan06.cn

Py:   from module import func
来源：http://kp.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cq.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://na.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kw.nszjky.cn

Java: import java.util.List;
来源：http://xr.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ul.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://tc.jctech888.com.cn

C#:   using System.Text;
来源：http://mg.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://nl.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://jc.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ol.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://bu.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://xc.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pn.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://rk.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://fj.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tf.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://bd.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zh.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://to.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tk.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yj.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nk.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://cr.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wg.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tj.haigaiapp.cn

[C14] 泛型函数
来源：http://vx.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fg.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://qv.bjjhwx.cn

JS:   // 无泛型
来源：http://qe.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://et.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vs.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gc.szsharing.cn

Ruby: # 无泛型
来源：http://bs.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kx.nszjky.cn

[C15] 解构 / 展开参数
来源：http://ny.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ep.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://lw.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kb.colortex.cn

Java: // 无解构
来源：http://zh.shxzskj.cn

Go:   // 无解构
来源：http://tb.hahajie.cn

Ruby: a, b = pair
来源：http://yc.9csxet.cn

C#:   var (a, b) = pair;
来源：http://hl.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://bh.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hr.haigaiapp.cn

PHP:  // 无重载
来源：http://gj.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uj.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://nc.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mr.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://nh.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://fg.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lg.bookmarksfly.cn

================================================================================
来源：http://ul.521024.cn

D. 数组 / 列表 / 集合
来源：http://np.szsharing.cn

================================================================================
来源：http://es.hahajie.cn

[D01] 创建数组 / 列表
来源：http://xg.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jc.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mk.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rw.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cp.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dt.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://ck.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ta.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gg.asd995.cn

[D02] 追加元素到末尾
来源：http://af.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cu.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ay.asd995.cn

TS:   arr.push(4);
来源：http://wt.bookmarksfly.cn

Java: list.add(4);
来源：http://to.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://wh.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://xx.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://li.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://rr.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://te.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ns.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oe.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://zq.shtwfgs.cn

Java: list.add(0, 0);
来源：http://vu.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hu.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ku.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://sd.bjjhwx.cn

[D04] 删除元素
来源：http://ss.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hv.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mk.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://pe.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ip.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xd.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ng.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://at.huixiangedu.cn

[D05] 访问与修改元素
来源：http://ed.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zg.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ps.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://cf.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://cy.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://id.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jo.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uh.huixiangedu.cn

[D06] 数组长度
来源：http://yk.chemitech.net.cn

Py:   len(arr)
来源：http://va.hnjuh.cn

PHP:  count($arr);
来源：http://ub.szsharing.cn

JS:   arr.length
来源：http://du.newstarts.cn

TS:   arr.length
来源：http://gu.huixinmuqiang.cn

Java: list.size();
来源：http://dq.jianghongdianzi.cn

Go:   len(arr)
来源：http://yj.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://mx.jianghongdianzi.cn

C#:   list.Count;
来源：http://ex.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://an.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ff.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qt.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://kr.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://xk.panjiajie.cn

Java: list.subList(1, 4);
来源：http://ub.gzmigu.cn

Go:   arr[1:4]
来源：http://lv.hahajie.cn

Ruby: arr[1, 3]
来源：http://pb.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://ih.9csxet.cn

[D08] 合并两个数组
来源：http://zu.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://pw.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://gi.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pv.shtwfgs.cn

TS:   [...a, ...b];
来源：http://uh.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yy.gzmigu.cn

Go:   append(a, b...)
来源：http://fu.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://vw.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://mr.9csxet.cn

[D09] 排序（升序）
来源：http://oe.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pb.gzmigu.cn

PHP:  sort($arr);
来源：http://or.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rb.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uu.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pk.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.nszjky.cn

Ruby: arr.sort
来源：http://sf.jctech888.com.cn

C#:   list.Sort();
来源：http://ub.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oy.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://us.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mb.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aq.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zi.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qu.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://go.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vi.newstarts.cn

[D11] 反转数组
来源：http://fy.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lr.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://kr.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jj.shxzukj.cn

TS:   [...arr].reverse();
来源：http://ql.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://au.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://js.lnxyls.cn

Ruby: arr.reverse
来源：http://ym.9csxet.cn

C#:   list.Reverse();
来源：http://zb.asd995.cn

[D12] 查找元素下标
来源：http://bu.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://fz.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qs.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wx.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zk.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hj.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://mt.asd995.cn

Ruby: arr.index(x)
来源：http://ku.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://uz.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://vj.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sk.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qo.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://km.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://ll.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vg.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ji.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://si.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ar.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://bp.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cb.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uq.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://iv.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://me.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yl.huixiangedu.cn

Go:   // 手写循环
来源：http://ys.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fw.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sz.huanxung.cn

[D15] 去重
来源：http://qo.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eu.asd995.cn

PHP:  array_unique($arr);
来源：http://fq.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://ij.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ic.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://em.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vt.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://js.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ql.nszjky.cn

[D16] 求和与平均值
来源：http://fk.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vk.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://re.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zm.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hh.521024.cn

Go:   // 手写循环累加
来源：http://zu.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bl.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://lf.hahajie.cn

[D17] 最大值与最小值
来源：http://al.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://ln.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://pn.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hc.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://kr.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hr.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lu.asd995.cn

Ruby: arr.max;  arr.min
来源：http://fq.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://qf.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ue.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qr.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://pn.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hs.lnxyls.cn

TS:   nested.flat();
来源：http://xy.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sl.haigaiapp.cn

Go:   // 手写双层循环
来源：http://wp.szsharing.cn

Ruby: nested.flatten
来源：http://pj.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yf.lnxyls.cn

[D19] 按字段分组
来源：http://bc.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kb.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://my.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ux.shtwfgs.cn


<!-- 参考信息 -->