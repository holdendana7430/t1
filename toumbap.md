代发 wailian999

Go:   a && b || !c
来源：http://ip.szsharing.cn

Ruby: a && b || !c
来源：http://fs.jianghongdianzi.cn

C#:   a && b || !c
来源：http://fk.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xz.huixinmuqiang.cn

Py:   if not data: return
来源：http://af.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://cl.szxytkj.cn

JS:   if (!data) return;
来源：http://lf.9csxet.cn

TS:   if (!data) return;
来源：http://xw.szxytkj.cn

Java: if (data == null) return;
来源：http://xh.hnjuh.cn

Go:   if data == nil { return }
来源：http://zl.shtwfgs.cn

Ruby: return if data.nil?
来源：http://dz.asd995.cn

C#:   if (data == null) return;
来源：http://xk.hahajie.cn

================================================================================
来源：http://sk.newstarts.cn

C. 函数与作用域
来源：http://jh.jianghongdianzi.cn

================================================================================
来源：http://pu.jianghongdianzi.cn

[C01] 定义函数
来源：http://dw.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://pj.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pf.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://uc.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sn.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nl.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ym.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://no.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hw.colortex.cn

[C02] 默认参数
来源：http://uw.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ic.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ip.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://bk.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jc.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lj.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yt.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ld.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://rn.nicolike.cn

[C03] 可变参数
来源：http://cc.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ik.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mb.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zx.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yf.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rv.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kl.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ue.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uy.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://sn.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dx.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pm.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ha.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nz.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://pd.521024.cn

Go:   // 无：用配置结构体参数
来源：http://ro.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://xv.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://mz.muxihuayi.cn

[C05] 返回多个值
来源：http://hy.yuexingan06.cn

Py:   return a, b
来源：http://gv.9csxet.cn

PHP:  return [$a, $b];
来源：http://ph.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gh.colortex.cn

TS:   return { a, b };
来源：http://bf.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ch.colortex.cn

Go:   return a, b
来源：http://md.huixiangedu.cn

Ruby: return a, b
来源：http://bq.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://mr.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://pl.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://wf.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ta.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://ru.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://fc.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cb.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mk.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://ta.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ry.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://wq.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ot.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vs.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zj.bookmarksfly.cn

TS:   arr.map(String)
来源：http://tc.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mf.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tl.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://lq.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qs.9csxet.cn

[C08] 闭包
来源：http://hs.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ft.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wq.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iy.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vv.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kb.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jm.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gi.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wl.muxihuayi.cn

[C09] 递归
来源：http://tn.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://th.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vj.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rv.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ec.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lz.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://os.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ts.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bt.panjiajie.cn

[C10] 变量作用域
来源：http://ku.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ql.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lu.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rs.jctech888.com.cn

TS:   同 JS
来源：http://ef.hahajie.cn

Java: 方法内为块级作用域
来源：http://sa.shtwfgs.cn

Go:   花括号块级作用域
来源：http://qx.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://np.szsharing.cn

C#:   块级作用域
来源：http://hg.shxzukj.cn

[C11] 模块导入与导出
来源：http://ic.newstarts.cn

Py:   from module import func
来源：http://ut.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://co.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hk.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lf.wgjwhj.cn

Java: import java.util.List;
来源：http://hn.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://do.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ai.jianghongdianzi.cn

C#:   using System.Text;
来源：http://vq.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://bs.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://bm.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://an.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://ew.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://lz.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bf.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://pc.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://yw.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qc.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://hs.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vm.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kl.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yn.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uk.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://po.nicolike.cn

Go:   func add(a, b int) int
来源：http://ky.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mx.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nl.wgjwhj.cn

[C14] 泛型函数
来源：http://gb.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rg.9csxet.cn

PHP:  // 无泛型
来源：http://gn.wgjwhj.cn

JS:   // 无泛型
来源：http://ir.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tc.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ek.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vu.nicolike.cn

Ruby: # 无泛型
来源：http://gr.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xj.521024.cn

[C15] 解构 / 展开参数
来源：http://gx.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eh.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://ho.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gt.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wr.colortex.cn

Java: // 无解构
来源：http://ak.shxzskj.cn

Go:   // 无解构
来源：http://xo.shxzskj.cn

Ruby: a, b = pair
来源：http://wy.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://oe.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://zf.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://be.hahajie.cn

PHP:  // 无重载
来源：http://pb.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tb.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://rg.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://by.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ey.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://ek.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rm.panjiajie.cn

================================================================================
来源：http://ll.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://xe.haigaiapp.cn

================================================================================
来源：http://wm.9csxet.cn

[D01] 创建数组 / 列表
来源：http://te.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ia.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nv.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xb.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ut.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rs.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://oh.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://rd.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hr.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ei.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xw.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lh.huanxung.cn

JS:   arr.push(4);
来源：http://og.szsharing.cn

TS:   arr.push(4);
来源：http://sl.szxytkj.cn

Java: list.add(4);
来源：http://sv.colortex.cn

Go:   arr = append(arr, 4)
来源：http://fw.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://bi.asd995.cn

C#:   list.Add(4);
来源：http://br.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://hs.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://nw.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vs.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yo.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ky.yuexingan06.cn

Java: list.add(0, 0);
来源：http://dh.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bx.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ns.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://cq.shtwfgs.cn

[D04] 删除元素
来源：http://jb.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qr.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://af.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://pn.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uy.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uh.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ro.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ez.szsharing.cn

[D05] 访问与修改元素
来源：http://vc.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mo.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nt.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ly.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://on.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ke.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nu.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cd.yuntaijiaju.cn

[D06] 数组长度
来源：http://tv.yuntaijiaju.cn

Py:   len(arr)
来源：http://ph.szxytkj.cn

PHP:  count($arr);
来源：http://oq.szxytkj.cn

JS:   arr.length
来源：http://en.colortex.cn

TS:   arr.length
来源：http://bl.yuexingan06.cn

Java: list.size();
来源：http://ck.haigaiapp.cn

Go:   len(arr)
来源：http://fx.colortex.cn

Ruby: arr.length; arr.size
来源：http://ec.yuexingan06.cn

C#:   list.Count;
来源：http://os.szsharing.cn

[D07] 切片 / 取子数组
来源：http://bx.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wn.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vz.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://fl.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://cq.newstarts.cn

Java: list.subList(1, 4);
来源：http://cx.shxzskj.cn

Go:   arr[1:4]
来源：http://eu.gzmigu.cn

Ruby: arr[1, 3]
来源：http://rv.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://hx.panjiajie.cn

[D08] 合并两个数组
来源：http://uz.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ta.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://xc.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pq.yuexingan06.cn

TS:   [...a, ...b];
来源：http://vz.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ja.hahajie.cn

Go:   append(a, b...)
来源：http://yp.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://jy.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://uh.muxihuayi.cn

[D09] 排序（升序）
来源：http://da.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://yg.shtwfgs.cn

PHP:  sort($arr);
来源：http://or.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ls.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ra.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hk.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ei.jctech888.com.cn

Ruby: arr.sort
来源：http://bg.shxzukj.cn

C#:   list.Sort();
来源：http://kf.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mg.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wy.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kp.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ii.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rg.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bg.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eq.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dn.bjjhwx.cn

[D11] 反转数组
来源：http://hw.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iq.asd995.cn

PHP:  array_reverse($arr);
来源：http://iv.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gf.newstarts.cn

TS:   [...arr].reverse();
来源：http://yn.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://nm.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://xu.9csxet.cn

Ruby: arr.reverse
来源：http://fk.nicolike.cn

C#:   list.Reverse();
来源：http://zc.panjiajie.cn

[D12] 查找元素下标
来源：http://ay.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://zi.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xl.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mv.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bp.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://sx.wgjwhj.cn

Ruby: arr.index(x)
来源：http://fb.521024.cn

C#:   list.IndexOf(x);
来源：http://qh.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://he.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qf.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ee.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://fn.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://gh.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ko.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ef.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ix.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cd.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://pi.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://na.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vg.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://el.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://zc.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://od.muxihuayi.cn

Go:   // 手写循环
来源：http://yp.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ka.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yt.szsharing.cn

[D15] 去重
来源：http://gn.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jx.hahajie.cn

PHP:  array_unique($arr);
来源：http://yf.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://dp.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://cd.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://at.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://op.hahajie.cn

Ruby: arr.uniq
来源：http://ia.521024.cn

C#:   list.Distinct().ToList()
来源：http://eu.wgjwhj.cn

[D16] 求和与平均值
来源：http://kh.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nt.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oa.huixinmuqiang.cn


<!-- 参考信息 -->