代发 wailian999

================================================================================
来源：http://mc.szsharing.cn

C. 函数与作用域
来源：http://rk.panjiajie.cn

================================================================================
来源：http://fw.shxzskj.cn

[C01] 定义函数
来源：http://pb.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://eh.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://nd.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sf.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://an.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mo.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://rp.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hq.szsharing.cn

[C02] 默认参数
来源：http://on.asd995.cn

Py:   def greet(name="World"): return name
来源：http://dj.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mj.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://xh.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dh.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qh.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dv.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://lg.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ay.wgjwhj.cn

[C03] 可变参数
来源：http://wm.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://aw.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fq.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fj.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xe.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ny.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uq.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uy.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pl.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://hr.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oq.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nq.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xb.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ft.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://xh.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ss.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://st.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://te.nszjky.cn

[C05] 返回多个值
来源：http://rg.haigaiapp.cn

Py:   return a, b
来源：http://zh.asd995.cn

PHP:  return [$a, $b];
来源：http://sp.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tc.nicolike.cn

TS:   return { a, b };
来源：http://kn.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sf.haigaiapp.cn

Go:   return a, b
来源：http://sd.hahajie.cn

Ruby: return a, b
来源：http://ty.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://rv.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://qx.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://er.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ce.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://tx.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://cb.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sv.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nu.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://qk.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lo.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ue.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://me.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cm.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ds.shxzukj.cn

TS:   arr.map(String)
来源：http://hh.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bm.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ai.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://mo.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tf.lnxyls.cn

[C08] 闭包
来源：http://qy.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lw.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yf.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tq.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mf.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://us.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aw.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wd.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ts.hahajie.cn

[C09] 递归
来源：http://vg.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jc.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xp.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lo.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lt.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://en.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bc.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pq.shtwfgs.cn

[C10] 变量作用域
来源：http://ee.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://js.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://se.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hy.newstarts.cn

TS:   同 JS
来源：http://wi.panjiajie.cn

Java: 方法内为块级作用域
来源：http://zm.shtwfgs.cn

Go:   花括号块级作用域
来源：http://dv.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ot.szsharing.cn

C#:   块级作用域
来源：http://ih.huanxung.cn

[C11] 模块导入与导出
来源：http://va.wgjwhj.cn

Py:   from module import func
来源：http://ys.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rs.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ed.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hs.nszjky.cn

Java: import java.util.List;
来源：http://rr.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iy.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ca.521024.cn

C#:   using System.Text;
来源：http://ma.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://jh.colortex.cn

Py:   (lambda: print("run"))()
来源：http://rg.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://bu.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://xt.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://pq.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kx.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://mp.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://jj.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wb.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://iw.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fk.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yo.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wx.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xd.newstarts.cn

Go:   func add(a, b int) int
来源：http://rc.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nb.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gt.szsharing.cn

[C14] 泛型函数
来源：http://mk.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vv.asd995.cn

PHP:  // 无泛型
来源：http://zv.bookmarksfly.cn

JS:   // 无泛型
来源：http://gt.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bs.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nb.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jn.haigaiapp.cn

Ruby: # 无泛型
来源：http://yr.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lw.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://tm.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aa.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://oh.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yh.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rf.muxihuayi.cn

Java: // 无解构
来源：http://yn.nicolike.cn

Go:   // 无解构
来源：http://mj.huanxung.cn

Ruby: a, b = pair
来源：http://ia.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ae.hahajie.cn

[C16] 函数 / 方法重载
来源：http://ld.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hl.nicolike.cn

PHP:  // 无重载
来源：http://lq.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fb.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://np.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ej.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://oc.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://hs.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vm.chemitech.net.cn

================================================================================
来源：http://pd.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://md.9csxet.cn

================================================================================
来源：http://xs.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://ll.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bf.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tk.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://er.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ra.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fo.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://mh.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://fm.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zs.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ap.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jm.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xh.szxytkj.cn

JS:   arr.push(4);
来源：http://cr.bookmarksfly.cn

TS:   arr.push(4);
来源：http://dc.521024.cn

Java: list.add(4);
来源：http://qi.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://fm.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://sx.haigaiapp.cn

C#:   list.Add(4);
来源：http://mn.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://nx.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://eu.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://no.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zt.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://mu.9csxet.cn

Java: list.add(0, 0);
来源：http://rp.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cw.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rm.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://dw.hahajie.cn

[D04] 删除元素
来源：http://pb.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lf.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://td.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nx.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://tb.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rw.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://df.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rc.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bc.huanxung.cn

[D05] 访问与修改元素
来源：http://er.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zb.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yi.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nd.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://zs.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://ts.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://lz.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ox.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pi.muxihuayi.cn

[D06] 数组长度
来源：http://cy.haigaiapp.cn

Py:   len(arr)
来源：http://jl.newstarts.cn

PHP:  count($arr);
来源：http://xe.bjjhwx.cn

JS:   arr.length
来源：http://bh.asd995.cn

TS:   arr.length
来源：http://hq.shxzukj.cn

Java: list.size();
来源：http://jd.asd995.cn

Go:   len(arr)
来源：http://dn.newstarts.cn

Ruby: arr.length; arr.size
来源：http://za.jctech888.com.cn

C#:   list.Count;
来源：http://gn.nicolike.cn

[D07] 切片 / 取子数组
来源：http://cz.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qb.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sq.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://sm.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://jx.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://me.huixiangedu.cn

Go:   arr[1:4]
来源：http://ap.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://qm.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://iy.newstarts.cn

[D08] 合并两个数组
来源：http://wl.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://qn.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://cd.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tn.szxytkj.cn

TS:   [...a, ...b];
来源：http://gi.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uc.gzmigu.cn

Go:   append(a, b...)
来源：http://tp.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://mz.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ar.huanxung.cn

[D09] 排序（升序）
来源：http://bh.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://ia.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://uv.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ch.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wi.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mf.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wh.nszjky.cn

Ruby: arr.sort
来源：http://nf.nszjky.cn

C#:   list.Sort();
来源：http://wi.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iq.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sn.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fy.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iv.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dw.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://za.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ov.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lo.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fp.huixinmuqiang.cn

[D11] 反转数组
来源：http://zi.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ut.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://or.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ds.szxytkj.cn

TS:   [...arr].reverse();
来源：http://gy.szxytkj.cn

Java: Collections.reverse(list);
来源：http://jr.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://gm.huanxung.cn

Ruby: arr.reverse
来源：http://gm.nicolike.cn

C#:   list.Reverse();
来源：http://sq.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://jy.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://is.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zz.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://px.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ay.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://au.asd995.cn

Go:   slices.Index(arr, x)
来源：http://wd.newstarts.cn

Ruby: arr.index(x)
来源：http://sy.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://rf.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://ei.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wa.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xy.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://jc.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://ws.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vq.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://md.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dc.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oe.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://oy.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oc.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rw.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://lz.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://po.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lm.szsharing.cn

Go:   // 手写循环
来源：http://ac.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ph.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xt.wgjwhj.cn

[D15] 去重
来源：http://kt.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yj.szsharing.cn

PHP:  array_unique($arr);
来源：http://qa.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://lx.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://pg.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qv.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ad.gzmigu.cn

Ruby: arr.uniq
来源：http://an.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://vi.gzmigu.cn

[D16] 求和与平均值
来源：http://qe.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nz.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iz.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cl.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ov.nszjky.cn

Go:   // 手写循环累加
来源：http://gx.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tq.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://zg.shtwfgs.cn

[D17] 最大值与最小值
来源：http://ec.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://yi.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ag.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dc.szxytkj.cn

TS:   Math.max(...arr);
来源：http://ij.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tn.chemitech.net.cn


<!-- 参考信息 -->