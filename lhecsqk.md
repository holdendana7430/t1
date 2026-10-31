代发 wailian999

Go:   a && b || !c
来源：http://xl.haigaiapp.cn

Ruby: a && b || !c
来源：http://oz.jctech888.com.cn

C#:   a && b || !c
来源：http://mg.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fq.lnxyls.cn

Py:   if not data: return
来源：http://na.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://gi.lnxyls.cn

JS:   if (!data) return;
来源：http://jl.lnxyls.cn

TS:   if (!data) return;
来源：http://dw.nicolike.cn

Java: if (data == null) return;
来源：http://lz.newstarts.cn

Go:   if data == nil { return }
来源：http://oc.huixiangedu.cn

Ruby: return if data.nil?
来源：http://hx.newstarts.cn

C#:   if (data == null) return;
来源：http://hl.yuntaijiaju.cn

================================================================================
来源：http://wh.chemitech.net.cn

C. 函数与作用域
来源：http://rs.panjiajie.cn

================================================================================
来源：http://rf.colortex.cn

[C01] 定义函数
来源：http://yr.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://jm.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tz.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://we.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cy.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ff.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ms.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://rh.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hw.huixiangedu.cn

[C02] 默认参数
来源：http://gb.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://am.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ae.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ro.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cz.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://da.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dg.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://sb.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://mj.9csxet.cn

[C03] 可变参数
来源：http://bj.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://nl.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wi.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vs.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nb.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ui.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sf.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tm.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nh.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://jw.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yq.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hx.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cu.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lw.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://br.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://wu.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://cj.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://vr.521024.cn

[C05] 返回多个值
来源：http://sc.shxzskj.cn

Py:   return a, b
来源：http://ys.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://mg.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fo.yuntaijiaju.cn

TS:   return { a, b };
来源：http://hb.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yx.newstarts.cn

Go:   return a, b
来源：http://li.panjiajie.cn

Ruby: return a, b
来源：http://te.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://vf.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://cs.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://kz.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://se.huanxung.cn

JS:   const square = x => x * x;
来源：http://cx.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ks.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nt.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yr.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ud.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qg.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://iw.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://la.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jh.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qg.nicolike.cn

TS:   arr.map(String)
来源：http://ko.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nz.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ko.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://bp.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://if.jianghongdianzi.cn

[C08] 闭包
来源：http://yo.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wz.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yc.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jj.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sc.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ad.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hl.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cl.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iz.nszjky.cn

[C09] 递归
来源：http://yy.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iu.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tw.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cj.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://td.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dt.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ig.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xc.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fo.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ea.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vv.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://di.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ae.asd995.cn

TS:   同 JS
来源：http://os.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://xt.nicolike.cn

Go:   花括号块级作用域
来源：http://cj.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yh.szxytkj.cn

C#:   块级作用域
来源：http://rt.shtwfgs.cn

[C11] 模块导入与导出
来源：http://cl.shtwfgs.cn

Py:   from module import func
来源：http://ta.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bn.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nv.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sw.chemitech.net.cn

Java: import java.util.List;
来源：http://vr.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wk.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://ku.jctech888.com.cn

C#:   using System.Text;
来源：http://cg.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://za.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://cg.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://eq.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ht.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://xj.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wp.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ip.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://nj.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dv.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://xo.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vv.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ku.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ba.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fr.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://db.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mz.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qo.bookmarksfly.cn

[C14] 泛型函数
来源：http://ca.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kf.bookmarksfly.cn

PHP:  // 无泛型
来源：http://xx.haigaiapp.cn

JS:   // 无泛型
来源：http://lv.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gc.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ye.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://du.hnjuh.cn

Ruby: # 无泛型
来源：http://ku.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://bi.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lf.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://lk.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vz.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qq.newstarts.cn

Java: // 无解构
来源：http://qf.shxzukj.cn

Go:   // 无解构
来源：http://fh.bjjhwx.cn

Ruby: a, b = pair
来源：http://ex.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://bi.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://tn.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qr.muxihuayi.cn

PHP:  // 无重载
来源：http://oy.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sw.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://jj.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bz.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://mn.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://ht.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sq.jctech888.com.cn

================================================================================
来源：http://ry.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://kh.colortex.cn

================================================================================
来源：http://ww.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://rs.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qt.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yn.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cb.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gr.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pq.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://tz.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://eg.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://to.shxzukj.cn

[D02] 追加元素到末尾
来源：http://pv.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ck.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yu.huanxung.cn

JS:   arr.push(4);
来源：http://cb.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://yu.9csxet.cn

Java: list.add(4);
来源：http://ey.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://jz.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://cv.huanxung.cn

C#:   list.Add(4);
来源：http://oz.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://sm.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://ga.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xz.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pa.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://ol.9csxet.cn

Java: list.add(0, 0);
来源：http://ft.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tn.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ns.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://dj.yuexingan06.cn

[D04] 删除元素
来源：http://we.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://br.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ss.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xl.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ik.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sf.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fo.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yn.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bo.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ct.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rt.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://at.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mv.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://fl.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://ax.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ow.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rs.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yr.huixinmuqiang.cn

[D06] 数组长度
来源：http://co.panjiajie.cn

Py:   len(arr)
来源：http://qd.huixiangedu.cn

PHP:  count($arr);
来源：http://mk.shxzskj.cn

JS:   arr.length
来源：http://uj.haigaiapp.cn

TS:   arr.length
来源：http://sa.huanxung.cn

Java: list.size();
来源：http://wn.wgjwhj.cn

Go:   len(arr)
来源：http://xn.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://qs.newstarts.cn

C#:   list.Count;
来源：http://ti.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://uw.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uq.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zc.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://as.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://in.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://kp.bookmarksfly.cn

Go:   arr[1:4]
来源：http://kn.szsharing.cn

Ruby: arr[1, 3]
来源：http://fc.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://wb.szsharing.cn

[D08] 合并两个数组
来源：http://pl.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://ef.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://dr.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xi.jctech888.com.cn

TS:   [...a, ...b];
来源：http://jz.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xz.szxytkj.cn

Go:   append(a, b...)
来源：http://id.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://si.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://wv.gzmigu.cn

[D09] 排序（升序）
来源：http://ab.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://qt.shtwfgs.cn

PHP:  sort($arr);
来源：http://ug.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sn.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ym.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tx.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bt.nicolike.cn

Ruby: arr.sort
来源：http://br.chemitech.net.cn

C#:   list.Sort();
来源：http://ut.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zu.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ia.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tw.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://id.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cc.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pj.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dq.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vi.wgjwhj.cn

[D11] 反转数组
来源：http://qw.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mz.colortex.cn

PHP:  array_reverse($arr);
来源：http://yt.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lw.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://bz.9csxet.cn

Java: Collections.reverse(list);
来源：http://np.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://bp.lnxyls.cn

Ruby: arr.reverse
来源：http://fq.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://sg.bookmarksfly.cn

[D12] 查找元素下标
来源：http://ep.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://qg.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ex.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jb.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wv.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ip.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ef.haigaiapp.cn

Ruby: arr.index(x)
来源：http://bv.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://sw.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://lc.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tj.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vb.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://lz.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ab.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hv.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cs.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cd.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lb.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://zs.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kc.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qt.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://oq.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://ui.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rf.shxzukj.cn

Go:   // 手写循环
来源：http://aq.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hp.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gs.bjjhwx.cn

[D15] 去重
来源：http://pr.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vz.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://oz.szsharing.cn

JS:   [...new Set(arr)]
来源：http://ri.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://du.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rl.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rr.shxzukj.cn

Ruby: arr.uniq
来源：http://jl.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://qp.shtwfgs.cn

[D16] 求和与平均值
来源：http://aw.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bj.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vr.panjiajie.cn


<!-- 参考信息 -->