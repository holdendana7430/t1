代发 wailian999

Java: if (data == null) return;
来源：http://wk.panjiajie.cn

Go:   if data == nil { return }
来源：http://ba.jctech888.com.cn

Ruby: return if data.nil?
来源：http://ky.jctech888.com.cn

C#:   if (data == null) return;
来源：http://az.yuntaijiaju.cn

================================================================================
来源：http://nc.haigaiapp.cn

C. 函数与作用域
来源：http://pf.hnjuh.cn

================================================================================
来源：http://gm.jianghongdianzi.cn

[C01] 定义函数
来源：http://lu.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://gc.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kp.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ge.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bz.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wd.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wt.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://ap.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gz.shtwfgs.cn

[C02] 默认参数
来源：http://wy.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://jt.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yr.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://wm.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rh.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bg.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ak.521024.cn

Ruby: def greet(name = "World") = name
来源：http://tw.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://mz.szxytkj.cn

[C03] 可变参数
来源：http://pj.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ek.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zv.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aw.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cq.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ke.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hb.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://es.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ub.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wi.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hg.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://iy.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://eu.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://dx.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://kc.hnjuh.cn

[C05] 返回多个值
来源：http://sz.haigaiapp.cn

Py:   return a, b
来源：http://as.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://ym.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aw.gzmigu.cn

TS:   return { a, b };
来源：http://bo.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gz.colortex.cn

Go:   return a, b
来源：http://ih.shxzskj.cn

Ruby: return a, b
来源：http://gz.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://rg.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ab.nszjky.cn

Py:   square = lambda x: x * x
来源：http://mm.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ze.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://xd.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://qp.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xs.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bk.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://oa.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sw.szsharing.cn

[C07] 把函数作为参数传入
来源：http://dh.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fr.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zv.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jg.shtwfgs.cn

TS:   arr.map(String)
来源：http://la.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jw.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pa.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://af.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ve.yuexingan06.cn

[C08] 闭包
来源：http://ho.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ax.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tp.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uq.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yp.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zd.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vr.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://co.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hm.521024.cn

[C09] 递归
来源：http://nj.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xi.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ca.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lw.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tr.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lu.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cl.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xr.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vj.asd995.cn

[C10] 变量作用域
来源：http://vg.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://la.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://di.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ey.hahajie.cn

TS:   同 JS
来源：http://eq.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://wa.colortex.cn

Go:   花括号块级作用域
来源：http://bk.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sw.szxytkj.cn

C#:   块级作用域
来源：http://ft.chemitech.net.cn

[C11] 模块导入与导出
来源：http://vh.nszjky.cn

Py:   from module import func
来源：http://aj.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aw.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pw.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yp.shtwfgs.cn

Java: import java.util.List;
来源：http://jy.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nv.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://wu.gzmigu.cn

C#:   using System.Text;
来源：http://fl.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://cu.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://do.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://pr.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://hz.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://dw.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qp.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://jj.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://oe.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ky.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://yh.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wc.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dq.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fs.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ud.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sp.szsharing.cn

Go:   func add(a, b int) int
来源：http://on.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qp.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ra.jianghongdianzi.cn

[C14] 泛型函数
来源：http://pz.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://um.hahajie.cn

PHP:  // 无泛型
来源：http://rh.panjiajie.cn

JS:   // 无泛型
来源：http://in.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pv.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pj.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mh.yuexingan06.cn

Ruby: # 无泛型
来源：http://dr.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://go.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://bd.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ux.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ji.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yo.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wd.colortex.cn

Java: // 无解构
来源：http://gp.hahajie.cn

Go:   // 无解构
来源：http://qt.lnxyls.cn

Ruby: a, b = pair
来源：http://gq.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://os.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://xc.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hr.nicolike.cn

PHP:  // 无重载
来源：http://aq.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gk.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://fy.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kj.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ei.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://fq.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gx.521024.cn

================================================================================
来源：http://nf.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://yd.bookmarksfly.cn

================================================================================
来源：http://ye.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://ej.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bb.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ie.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ma.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sn.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xm.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://xm.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://pw.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bh.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ax.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://op.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dt.hahajie.cn

JS:   arr.push(4);
来源：http://di.chemitech.net.cn

TS:   arr.push(4);
来源：http://ve.panjiajie.cn

Java: list.add(4);
来源：http://nf.asd995.cn

Go:   arr = append(arr, 4)
来源：http://qv.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://vb.newstarts.cn

C#:   list.Add(4);
来源：http://qk.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://wv.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ca.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xd.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://id.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://mi.521024.cn

Java: list.add(0, 0);
来源：http://ol.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zn.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vz.colortex.cn

C#:   list.Insert(0, 0);
来源：http://el.9csxet.cn

[D04] 删除元素
来源：http://lk.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ad.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rs.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vd.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://vf.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qj.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qz.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zd.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rb.szxytkj.cn

[D05] 访问与修改元素
来源：http://ej.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gb.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bb.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wr.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://ly.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://xi.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://fq.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hk.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zj.panjiajie.cn

[D06] 数组长度
来源：http://yj.newstarts.cn

Py:   len(arr)
来源：http://qu.bjjhwx.cn

PHP:  count($arr);
来源：http://bq.jctech888.com.cn

JS:   arr.length
来源：http://mk.nszjky.cn

TS:   arr.length
来源：http://qx.bjjhwx.cn

Java: list.size();
来源：http://nc.521024.cn

Go:   len(arr)
来源：http://jl.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://ul.shxzskj.cn

C#:   list.Count;
来源：http://fc.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://xn.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rb.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ya.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://pk.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://ib.szsharing.cn

Java: list.subList(1, 4);
来源：http://wj.yuexingan06.cn

Go:   arr[1:4]
来源：http://uy.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://kb.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://es.newstarts.cn

[D08] 合并两个数组
来源：http://pv.521024.cn

Py:   a + b;  a.extend(b)
来源：http://vo.colortex.cn

PHP:  array_merge($a, $b);
来源：http://kj.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vn.shxzskj.cn

TS:   [...a, ...b];
来源：http://pw.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fh.bookmarksfly.cn

Go:   append(a, b...)
来源：http://so.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://vv.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://od.huanxung.cn

[D09] 排序（升序）
来源：http://kj.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://xd.yuexingan06.cn

PHP:  sort($arr);
来源：http://zv.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fk.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qr.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kb.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bt.yuexingan06.cn

Ruby: arr.sort
来源：http://nm.huixiangedu.cn

C#:   list.Sort();
来源：http://oo.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qi.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qr.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mg.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fv.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xx.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bn.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bs.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ze.521024.cn

[D11] 反转数组
来源：http://rp.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pl.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://pb.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://je.nszjky.cn

TS:   [...arr].reverse();
来源：http://er.huanxung.cn

Java: Collections.reverse(list);
来源：http://wo.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://gb.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ta.bookmarksfly.cn

C#:   list.Reverse();
来源：http://es.szsharing.cn

[D12] 查找元素下标
来源：http://zo.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://vj.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ox.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ix.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://re.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uh.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://vs.muxihuayi.cn

Ruby: arr.index(x)
来源：http://kx.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ff.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://ep.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ni.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sl.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://jo.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://hl.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qd.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pp.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://im.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lz.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://go.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bw.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gd.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://bq.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://pb.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mu.shxzskj.cn

Go:   // 手写循环
来源：http://nb.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mh.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://la.nszjky.cn

[D15] 去重
来源：http://wn.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xb.521024.cn

PHP:  array_unique($arr);
来源：http://fl.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://fd.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://co.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nj.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pt.nicolike.cn

Ruby: arr.uniq
来源：http://bl.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://hg.wgjwhj.cn

[D16] 求和与平均值
来源：http://pb.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lw.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aq.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gu.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://on.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jo.haigaiapp.cn

Go:   // 手写循环累加
来源：http://hb.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vv.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://pe.szxytkj.cn

[D17] 最大值与最小值
来源：http://ha.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://xx.hahajie.cn


<!-- 参考信息 -->