代发 wailian999

PHP:  $a && $b || !$c
来源：http://kd.chemitech.net.cn

JS:   a && b || !c
来源：http://li.colortex.cn

TS:   a && b || !c
来源：http://dd.lnxyls.cn

Java: a && b || !c
来源：http://ok.muxihuayi.cn

Go:   a && b || !c
来源：http://za.shxzskj.cn

Ruby: a && b || !c
来源：http://mo.huixiangedu.cn

C#:   a && b || !c
来源：http://gm.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zl.chemitech.net.cn

Py:   if not data: return
来源：http://eb.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://hn.bookmarksfly.cn

JS:   if (!data) return;
来源：http://fz.gzmigu.cn

TS:   if (!data) return;
来源：http://aa.chemitech.net.cn

Java: if (data == null) return;
来源：http://wb.shtwfgs.cn

Go:   if data == nil { return }
来源：http://du.nszjky.cn

Ruby: return if data.nil?
来源：http://ys.gzmigu.cn

C#:   if (data == null) return;
来源：http://ir.lnxyls.cn

================================================================================
来源：http://fe.huixiangedu.cn

C. 函数与作用域
来源：http://az.wgjwhj.cn

================================================================================
来源：http://yn.huixiangedu.cn

[C01] 定义函数
来源：http://qd.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://fu.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xj.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gg.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mp.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zp.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ph.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rw.jctech888.com.cn

[C02] 默认参数
来源：http://yl.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://hk.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://my.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://he.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mg.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mu.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sv.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://pi.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://rl.jctech888.com.cn

[C03] 可变参数
来源：http://ou.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://ax.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://or.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ni.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://od.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mu.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dc.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gr.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sw.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://rk.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oa.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yu.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xk.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://np.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://eq.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://se.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://vr.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://lq.yuexingan06.cn

[C05] 返回多个值
来源：http://bm.szxytkj.cn

Py:   return a, b
来源：http://kf.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://ga.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wa.muxihuayi.cn

TS:   return { a, b };
来源：http://pa.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bh.chemitech.net.cn

Go:   return a, b
来源：http://xa.hnjuh.cn

Ruby: return a, b
来源：http://vi.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://qe.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://vz.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ns.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rc.521024.cn

JS:   const square = x => x * x;
来源：http://xc.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://dj.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yn.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dk.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://vw.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tx.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://vt.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qh.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xc.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.hahajie.cn

TS:   arr.map(String)
来源：http://nf.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ir.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ct.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://ya.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jr.bookmarksfly.cn

[C08] 闭包
来源：http://qh.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jd.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://li.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dg.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fx.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qx.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://li.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fn.szsharing.cn

[C09] 递归
来源：http://dt.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bi.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pm.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qr.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sw.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://by.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bv.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cg.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xa.shxzskj.cn

[C10] 变量作用域
来源：http://xt.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ht.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ag.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jb.szsharing.cn

TS:   同 JS
来源：http://qi.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://iq.hahajie.cn

Go:   花括号块级作用域
来源：http://ja.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oo.9csxet.cn

C#:   块级作用域
来源：http://za.panjiajie.cn

[C11] 模块导入与导出
来源：http://fv.yuexingan06.cn

Py:   from module import func
来源：http://wo.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://um.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kv.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tv.haigaiapp.cn

Java: import java.util.List;
来源：http://si.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ud.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ns.newstarts.cn

C#:   using System.Text;
来源：http://uj.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ll.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://tj.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://bg.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://se.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://xe.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kj.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://rb.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://hf.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dq.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://aa.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qv.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kf.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://py.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lv.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qo.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://zn.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hl.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rp.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ay.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://en.jctech888.com.cn

PHP:  // 无泛型
来源：http://ml.chemitech.net.cn

JS:   // 无泛型
来源：http://vm.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qf.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eq.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xc.szsharing.cn

Ruby: # 无泛型
来源：http://hj.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://th.521024.cn

[C15] 解构 / 展开参数
来源：http://mo.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://in.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://ux.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hl.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tk.hahajie.cn

Java: // 无解构
来源：http://vl.hahajie.cn

Go:   // 无解构
来源：http://sl.jctech888.com.cn

Ruby: a, b = pair
来源：http://yv.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://eu.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://zn.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lp.newstarts.cn

PHP:  // 无重载
来源：http://ff.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fw.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://mj.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kz.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://fg.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://gd.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tn.szsharing.cn

================================================================================
来源：http://mx.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://jv.nicolike.cn

================================================================================
来源：http://qd.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://lm.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tx.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pf.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cj.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://km.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tn.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://qc.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://pq.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hx.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://gz.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xm.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pr.nszjky.cn

JS:   arr.push(4);
来源：http://yl.9csxet.cn

TS:   arr.push(4);
来源：http://ee.asd995.cn

Java: list.add(4);
来源：http://yv.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://ea.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://hd.asd995.cn

C#:   list.Add(4);
来源：http://wz.huanxung.cn

[D03] 在指定位置插入元素
来源：http://ov.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://lc.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hk.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tv.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://wr.szsharing.cn

Java: list.add(0, 0);
来源：http://dj.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://er.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ic.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ia.newstarts.cn

[D04] 删除元素
来源：http://zo.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xg.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ey.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://om.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://fn.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tx.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dt.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qc.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lk.chemitech.net.cn

[D05] 访问与修改元素
来源：http://yb.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ek.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bq.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pu.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://pi.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ir.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://si.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ta.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jq.jianghongdianzi.cn

[D06] 数组长度
来源：http://by.nicolike.cn

Py:   len(arr)
来源：http://ke.yuntaijiaju.cn

PHP:  count($arr);
来源：http://bf.shtwfgs.cn

JS:   arr.length
来源：http://re.huixinmuqiang.cn

TS:   arr.length
来源：http://gi.muxihuayi.cn

Java: list.size();
来源：http://wd.gzmigu.cn

Go:   len(arr)
来源：http://wm.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://hl.muxihuayi.cn

C#:   list.Count;
来源：http://mx.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ya.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sb.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zh.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://lr.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://kr.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://sy.bjjhwx.cn

Go:   arr[1:4]
来源：http://xo.lnxyls.cn

Ruby: arr[1, 3]
来源：http://vo.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://bq.huixiangedu.cn

[D08] 合并两个数组
来源：http://pk.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://rr.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://rz.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nr.hnjuh.cn

TS:   [...a, ...b];
来源：http://yi.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tf.bjjhwx.cn

Go:   append(a, b...)
来源：http://is.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://xy.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ez.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://va.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://rj.jctech888.com.cn

PHP:  sort($arr);
来源：http://zz.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hm.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sc.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vd.huanxung.cn

Ruby: arr.sort
来源：http://zt.yuntaijiaju.cn

C#:   list.Sort();
来源：http://xo.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ba.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vo.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zn.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://id.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ay.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pz.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://no.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tn.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ew.newstarts.cn

[D11] 反转数组
来源：http://me.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kb.nszjky.cn

PHP:  array_reverse($arr);
来源：http://zb.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uw.gzmigu.cn

TS:   [...arr].reverse();
来源：http://vy.panjiajie.cn

Java: Collections.reverse(list);
来源：http://yl.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://fk.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ph.shxzskj.cn

C#:   list.Reverse();
来源：http://qf.shxzskj.cn

[D12] 查找元素下标
来源：http://dp.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://sf.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dv.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kd.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mr.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ql.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://io.newstarts.cn

Ruby: arr.index(x)
来源：http://wn.huanxung.cn

C#:   list.IndexOf(x);
来源：http://ih.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://of.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yn.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://pt.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ae.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://re.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eg.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rc.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://me.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://ux.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uy.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bo.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://um.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://ep.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qi.lnxyls.cn

Go:   // 手写循环
来源：http://la.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lz.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kq.gzmigu.cn

[D15] 去重
来源：http://lb.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hg.521024.cn

PHP:  array_unique($arr);
来源：http://ot.szsharing.cn

JS:   [...new Set(arr)]
来源：http://pa.521024.cn

TS:   [...new Set(arr)]
来源：http://mp.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fb.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lw.szsharing.cn

Ruby: arr.uniq
来源：http://ix.huanxung.cn


<!-- 参考信息 -->