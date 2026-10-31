代发 wailian999

Java: if (data == null) return;
来源：http://od.hahajie.cn

Go:   if data == nil { return }
来源：http://gi.9csxet.cn

Ruby: return if data.nil?
来源：http://hy.muxihuayi.cn

C#:   if (data == null) return;
来源：http://yb.nicolike.cn

================================================================================
来源：http://jf.9csxet.cn

C. 函数与作用域
来源：http://kf.szsharing.cn

================================================================================
来源：http://uq.hnjuh.cn

[C01] 定义函数
来源：http://pm.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://sv.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jt.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://jr.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://se.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ra.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wi.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://bx.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sn.shxzukj.cn

[C02] 默认参数
来源：http://du.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://kf.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ks.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yg.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jq.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vk.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ni.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jp.521024.cn

[C03] 可变参数
来源：http://ps.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://su.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qe.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://km.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://np.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xx.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uq.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://db.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bt.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://gr.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jo.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tp.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hx.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jv.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://pb.521024.cn

Go:   // 无：用配置结构体参数
来源：http://wl.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://ia.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://wy.asd995.cn

[C05] 返回多个值
来源：http://ht.yuexingan06.cn

Py:   return a, b
来源：http://lc.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://lb.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ml.colortex.cn

TS:   return { a, b };
来源：http://wp.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ge.bookmarksfly.cn

Go:   return a, b
来源：http://iw.yuntaijiaju.cn

Ruby: return a, b
来源：http://xv.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://pw.521024.cn

[C06] 匿名函数 / lambda
来源：http://tr.9csxet.cn

Py:   square = lambda x: x * x
来源：http://kw.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zf.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://xd.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://uq.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bk.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ja.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://zs.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.huanxung.cn

[C07] 把函数作为参数传入
来源：http://pt.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://op.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uy.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dp.asd995.cn

TS:   arr.map(String)
来源：http://zr.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://az.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://av.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ll.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://du.jianghongdianzi.cn

[C08] 闭包
来源：http://rs.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lt.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xr.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zk.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ti.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bz.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zq.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eu.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ql.huanxung.cn

[C09] 递归
来源：http://as.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rv.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xl.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kt.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ip.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bu.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ip.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cc.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ru.521024.cn

[C10] 变量作用域
来源：http://ji.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tv.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://we.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nm.nszjky.cn

TS:   同 JS
来源：http://wa.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://um.nszjky.cn

Go:   花括号块级作用域
来源：http://sp.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qv.huixiangedu.cn

C#:   块级作用域
来源：http://ok.9csxet.cn

[C11] 模块导入与导出
来源：http://xb.asd995.cn

Py:   from module import func
来源：http://iq.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bt.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bi.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ey.jctech888.com.cn

Java: import java.util.List;
来源：http://rs.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zy.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://hz.shtwfgs.cn

C#:   using System.Text;
来源：http://fv.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://kl.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://hk.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://yb.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://xn.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://te.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zy.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://dk.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ei.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pg.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ro.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sj.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://af.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vc.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kq.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ay.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://th.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ou.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ja.szsharing.cn

[C14] 泛型函数
来源：http://bl.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://up.huixiangedu.cn

PHP:  // 无泛型
来源：http://to.shxzukj.cn

JS:   // 无泛型
来源：http://cu.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lb.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dw.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ov.shxzskj.cn

Ruby: # 无泛型
来源：http://sz.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ay.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://gd.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bm.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://yp.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jm.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mj.shxzskj.cn

Java: // 无解构
来源：http://gv.lnxyls.cn

Go:   // 无解构
来源：http://is.nicolike.cn

Ruby: a, b = pair
来源：http://eq.asd995.cn

C#:   var (a, b) = pair;
来源：http://kt.colortex.cn

[C16] 函数 / 方法重载
来源：http://sl.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yt.nicolike.cn

PHP:  // 无重载
来源：http://dj.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xu.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jm.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://zw.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://kq.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cf.muxihuayi.cn

================================================================================
来源：http://ml.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://jd.muxihuayi.cn

================================================================================
来源：http://dl.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://pb.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zk.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ci.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://it.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ae.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yt.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ql.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ex.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fx.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://tc.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yw.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://un.hahajie.cn

JS:   arr.push(4);
来源：http://nj.hahajie.cn

TS:   arr.push(4);
来源：http://lx.gzmigu.cn

Java: list.add(4);
来源：http://nr.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://ko.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ra.haigaiapp.cn

C#:   list.Add(4);
来源：http://qo.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ms.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://br.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ou.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://un.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://kr.jctech888.com.cn

Java: list.add(0, 0);
来源：http://ac.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://en.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ck.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://jb.nicolike.cn

[D04] 删除元素
来源：http://nt.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vf.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yu.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vr.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://rl.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jm.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lh.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ga.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vj.huixiangedu.cn

[D05] 访问与修改元素
来源：http://kq.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lw.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fk.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lo.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://cy.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://gs.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ah.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nd.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bb.shxzukj.cn

[D06] 数组长度
来源：http://xp.haigaiapp.cn

Py:   len(arr)
来源：http://sq.asd995.cn

PHP:  count($arr);
来源：http://dq.panjiajie.cn

JS:   arr.length
来源：http://ud.gzmigu.cn

TS:   arr.length
来源：http://xr.nszjky.cn

Java: list.size();
来源：http://zo.huanxung.cn

Go:   len(arr)
来源：http://kj.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://pj.muxihuayi.cn

C#:   list.Count;
来源：http://ll.nicolike.cn

[D07] 切片 / 取子数组
来源：http://br.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rg.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://un.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://il.colortex.cn

TS:   arr.slice(1, 4);
来源：http://sn.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://rp.colortex.cn

Go:   arr[1:4]
来源：http://xz.521024.cn

Ruby: arr[1, 3]
来源：http://cg.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://rb.wgjwhj.cn

[D08] 合并两个数组
来源：http://fh.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://ou.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://zp.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ea.newstarts.cn

TS:   [...a, ...b];
来源：http://ih.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ac.szxytkj.cn

Go:   append(a, b...)
来源：http://jp.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://uj.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://za.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://fs.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://cs.panjiajie.cn

PHP:  sort($arr);
来源：http://vd.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ui.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://at.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kc.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bw.9csxet.cn

Ruby: arr.sort
来源：http://oo.jctech888.com.cn

C#:   list.Sort();
来源：http://aw.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yt.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ps.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hn.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pi.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hf.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rp.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wq.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yk.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ye.nicolike.cn

[D11] 反转数组
来源：http://al.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://np.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://wm.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sp.hnjuh.cn

TS:   [...arr].reverse();
来源：http://fn.asd995.cn

Java: Collections.reverse(list);
来源：http://jo.asd995.cn

Go:   slices.Reverse(arr)
来源：http://fd.lnxyls.cn

Ruby: arr.reverse
来源：http://mf.bjjhwx.cn

C#:   list.Reverse();
来源：http://ko.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://dx.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://lm.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wf.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lt.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hy.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gz.asd995.cn

Go:   slices.Index(arr, x)
来源：http://nc.shtwfgs.cn

Ruby: arr.index(x)
来源：http://vg.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://xe.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://dr.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://if.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xg.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://mj.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://uq.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mb.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mi.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dd.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hj.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://vc.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wo.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ma.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ut.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://vr.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nc.haigaiapp.cn

Go:   // 手写循环
来源：http://fc.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yx.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ol.jianghongdianzi.cn

[D15] 去重
来源：http://sp.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zp.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://ws.colortex.cn

JS:   [...new Set(arr)]
来源：http://yz.hahajie.cn

TS:   [...new Set(arr)]
来源：http://py.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wg.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qo.panjiajie.cn

Ruby: arr.uniq
来源：http://ja.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ko.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://rx.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gu.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zi.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tl.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lh.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tt.shtwfgs.cn

Go:   // 手写循环累加
来源：http://ks.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kc.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://jg.nicolike.cn

[D17] 最大值与最小值
来源：http://bz.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://cy.chemitech.net.cn


<!-- 参考信息 -->