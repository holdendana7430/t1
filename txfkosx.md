代发 wailian999

Java: if (data == null) return;
来源：http://bh.huixiangedu.cn

Go:   if data == nil { return }
来源：http://cd.colortex.cn

Ruby: return if data.nil?
来源：http://km.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ur.hnjuh.cn

================================================================================
来源：http://sy.muxihuayi.cn

C. 函数与作用域
来源：http://ew.huixiangedu.cn

================================================================================
来源：http://va.panjiajie.cn

[C01] 定义函数
来源：http://az.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://pa.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://id.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://mn.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ot.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fr.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ir.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://kp.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rv.hahajie.cn

[C02] 默认参数
来源：http://tq.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://aq.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ey.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://es.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ak.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sp.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qn.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://yn.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://kl.lnxyls.cn

[C03] 可变参数
来源：http://cz.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://iv.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zt.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tc.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://js.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pz.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ik.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vz.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xw.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://fh.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rq.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qo.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cn.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rs.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://ey.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://aj.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://lm.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://iw.bjjhwx.cn

[C05] 返回多个值
来源：http://mj.asd995.cn

Py:   return a, b
来源：http://mg.9csxet.cn

PHP:  return [$a, $b];
来源：http://vc.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yh.wgjwhj.cn

TS:   return { a, b };
来源：http://xw.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xd.jianghongdianzi.cn

Go:   return a, b
来源：http://vj.521024.cn

Ruby: return a, b
来源：http://ij.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xv.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://uu.huanxung.cn

Py:   square = lambda x: x * x
来源：http://mf.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vx.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://zn.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://bb.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bx.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ai.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://zd.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ee.9csxet.cn

[C07] 把函数作为参数传入
来源：http://wz.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qf.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qa.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zk.haigaiapp.cn

TS:   arr.map(String)
来源：http://if.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pp.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nh.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://zn.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ji.panjiajie.cn

[C08] 闭包
来源：http://dx.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gm.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fw.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ul.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fh.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nq.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mp.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jr.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bw.jctech888.com.cn

[C09] 递归
来源：http://ut.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yw.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vb.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sk.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ar.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tt.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fc.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://up.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wg.szsharing.cn

[C10] 变量作用域
来源：http://ev.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rz.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sw.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://it.haigaiapp.cn

TS:   同 JS
来源：http://sd.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ji.yuexingan06.cn

Go:   花括号块级作用域
来源：http://vt.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gu.huixiangedu.cn

C#:   块级作用域
来源：http://ij.shtwfgs.cn

[C11] 模块导入与导出
来源：http://bb.szsharing.cn

Py:   from module import func
来源：http://ot.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dl.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rd.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ns.szxytkj.cn

Java: import java.util.List;
来源：http://oz.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bd.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://nf.haigaiapp.cn

C#:   using System.Text;
来源：http://hk.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://zk.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://xa.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://go.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://km.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ap.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://io.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vc.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://as.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wp.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://wx.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tb.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kd.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cp.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://it.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lr.hahajie.cn

Go:   func add(a, b int) int
来源：http://ej.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sh.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ld.shtwfgs.cn

[C14] 泛型函数
来源：http://bk.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mj.9csxet.cn

PHP:  // 无泛型
来源：http://yt.newstarts.cn

JS:   // 无泛型
来源：http://ea.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rl.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nx.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bz.colortex.cn

Ruby: # 无泛型
来源：http://ot.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fn.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://et.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cx.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://oe.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://en.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hd.szsharing.cn

Java: // 无解构
来源：http://hy.asd995.cn

Go:   // 无解构
来源：http://ct.nicolike.cn

Ruby: a, b = pair
来源：http://dv.9csxet.cn

C#:   var (a, b) = pair;
来源：http://hr.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://lv.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vn.nszjky.cn

PHP:  // 无重载
来源：http://tl.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ih.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ga.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sm.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://ej.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://sg.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ma.haigaiapp.cn

================================================================================
来源：http://ur.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://pi.huixinmuqiang.cn

================================================================================
来源：http://qz.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ae.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ah.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gy.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uu.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://np.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mj.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://op.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://pw.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://er.hnjuh.cn

[D02] 追加元素到末尾
来源：http://zd.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lp.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yy.wgjwhj.cn

JS:   arr.push(4);
来源：http://rc.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://sp.muxihuayi.cn

Java: list.add(4);
来源：http://nq.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://kw.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://dt.wgjwhj.cn

C#:   list.Add(4);
来源：http://bz.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ui.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://wc.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yp.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fl.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ls.shxzskj.cn

Java: list.add(0, 0);
来源：http://qc.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wm.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rh.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://bi.shtwfgs.cn

[D04] 删除元素
来源：http://sw.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xg.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zz.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yh.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://ml.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vy.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rj.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gq.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lb.newstarts.cn

[D05] 访问与修改元素
来源：http://ky.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tv.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yj.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nj.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://rk.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://uj.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://um.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qn.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lb.nicolike.cn

[D06] 数组长度
来源：http://fa.nszjky.cn

Py:   len(arr)
来源：http://sq.panjiajie.cn

PHP:  count($arr);
来源：http://jt.wgjwhj.cn

JS:   arr.length
来源：http://bm.lnxyls.cn

TS:   arr.length
来源：http://eh.huixinmuqiang.cn

Java: list.size();
来源：http://md.panjiajie.cn

Go:   len(arr)
来源：http://ox.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://xj.muxihuayi.cn

C#:   list.Count;
来源：http://br.asd995.cn

[D07] 切片 / 取子数组
来源：http://xm.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yd.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wo.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://jl.colortex.cn

TS:   arr.slice(1, 4);
来源：http://nu.gzmigu.cn

Java: list.subList(1, 4);
来源：http://ja.panjiajie.cn

Go:   arr[1:4]
来源：http://ac.hahajie.cn

Ruby: arr[1, 3]
来源：http://nh.521024.cn

C#:   list.GetRange(1, 3);
来源：http://vs.colortex.cn

[D08] 合并两个数组
来源：http://pz.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://ma.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://sw.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fi.wgjwhj.cn

TS:   [...a, ...b];
来源：http://it.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lz.gzmigu.cn

Go:   append(a, b...)
来源：http://ag.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://xz.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://lv.chemitech.net.cn

[D09] 排序（升序）
来源：http://ln.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://jz.gzmigu.cn

PHP:  sort($arr);
来源：http://rn.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ab.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nd.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tm.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dr.newstarts.cn

Ruby: arr.sort
来源：http://bl.nszjky.cn

C#:   list.Sort();
来源：http://ek.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dm.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ra.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cp.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ar.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yb.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bm.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ka.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zl.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ih.muxihuayi.cn

[D11] 反转数组
来源：http://ih.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yk.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ge.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rd.panjiajie.cn

TS:   [...arr].reverse();
来源：http://lv.shxzukj.cn

Java: Collections.reverse(list);
来源：http://hm.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ku.shxzskj.cn

Ruby: arr.reverse
来源：http://oz.newstarts.cn

C#:   list.Reverse();
来源：http://pb.haigaiapp.cn

[D12] 查找元素下标
来源：http://zr.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://cu.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ao.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iw.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://os.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ag.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ao.jctech888.com.cn

Ruby: arr.index(x)
来源：http://qv.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://id.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://nn.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hg.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yp.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://si.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://uw.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gq.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ov.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tg.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://bw.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qk.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://eg.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://ak.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ti.huanxung.cn

Go:   // 手写循环
来源：http://jk.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sm.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bk.shxzukj.cn

[D15] 去重
来源：http://mz.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ka.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://vp.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://qw.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://mc.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sd.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fr.9csxet.cn

Ruby: arr.uniq
来源：http://hz.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://zg.shxzskj.cn

[D16] 求和与平均值
来源：http://wq.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uz.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zi.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gd.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tr.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xg.chemitech.net.cn

Go:   // 手写循环累加
来源：http://xz.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gu.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://nf.newstarts.cn

[D17] 最大值与最小值
来源：http://iz.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://mr.chemitech.net.cn


<!-- 参考信息 -->