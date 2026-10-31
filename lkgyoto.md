代发 wailian999

Go:   a && b || !c
来源：http://pv.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://sa.huixiangedu.cn

C#:   a && b || !c
来源：http://lv.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oi.jctech888.com.cn

Py:   if not data: return
来源：http://tf.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://ig.shxzskj.cn

JS:   if (!data) return;
来源：http://kh.nszjky.cn

TS:   if (!data) return;
来源：http://kc.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://tr.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://kc.521024.cn

Ruby: return if data.nil?
来源：http://lo.huixiangedu.cn

C#:   if (data == null) return;
来源：http://mb.nszjky.cn

================================================================================
来源：http://iz.shtwfgs.cn

C. 函数与作用域
来源：http://rq.szxytkj.cn

================================================================================
来源：http://re.asd995.cn

[C01] 定义函数
来源：http://ti.colortex.cn

Py:   def add(a, b): return a + b
来源：http://nz.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sm.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://df.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pt.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bi.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ln.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ni.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gs.nszjky.cn

[C02] 默认参数
来源：http://ew.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://ph.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sy.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://pr.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qt.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dm.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://qz.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://qu.szsharing.cn

[C03] 可变参数
来源：http://an.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://xv.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://og.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vy.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ao.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vf.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ts.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tx.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://mk.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dj.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cw.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hp.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jo.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ya.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://xu.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://qs.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://dw.huixiangedu.cn

[C05] 返回多个值
来源：http://gp.bjjhwx.cn

Py:   return a, b
来源：http://cj.panjiajie.cn

PHP:  return [$a, $b];
来源：http://xu.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rk.lnxyls.cn

TS:   return { a, b };
来源：http://wp.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vg.9csxet.cn

Go:   return a, b
来源：http://pi.shtwfgs.cn

Ruby: return a, b
来源：http://cn.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://vz.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://sq.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://hr.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dj.nicolike.cn

JS:   const square = x => x * x;
来源：http://ku.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://vi.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mb.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qo.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://zz.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nf.nszjky.cn

[C07] 把函数作为参数传入
来源：http://wo.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ik.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bq.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ak.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://tp.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lp.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://is.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://sj.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yw.gzmigu.cn

[C08] 闭包
来源：http://gs.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ui.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nn.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://um.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wx.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bi.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bk.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ot.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zj.panjiajie.cn

[C09] 递归
来源：http://jz.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qm.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jl.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ik.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oi.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ul.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hg.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cf.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ur.hnjuh.cn

[C10] 变量作用域
来源：http://vo.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yd.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lm.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tp.yuexingan06.cn

TS:   同 JS
来源：http://wb.521024.cn

Java: 方法内为块级作用域
来源：http://mp.yuexingan06.cn

Go:   花括号块级作用域
来源：http://kb.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://al.haigaiapp.cn

C#:   块级作用域
来源：http://ff.asd995.cn

[C11] 模块导入与导出
来源：http://du.bookmarksfly.cn

Py:   from module import func
来源：http://ot.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fo.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xn.asd995.cn

Java: import java.util.List;
来源：http://wr.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dy.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://rm.bookmarksfly.cn

C#:   using System.Text;
来源：http://xc.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://kb.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://gt.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://io.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://li.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://jm.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vq.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ll.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://gk.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ey.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://iv.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jl.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://va.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qj.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ie.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pr.hahajie.cn

Go:   func add(a, b int) int
来源：http://oe.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wx.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lv.yuntaijiaju.cn

[C14] 泛型函数
来源：http://xf.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xj.bjjhwx.cn

PHP:  // 无泛型
来源：http://ts.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pv.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lm.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ma.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rr.gzmigu.cn

Ruby: # 无泛型
来源：http://xk.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ay.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://bf.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ia.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://lx.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ht.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wn.newstarts.cn

Java: // 无解构
来源：http://rm.colortex.cn

Go:   // 无解构
来源：http://sl.9csxet.cn

Ruby: a, b = pair
来源：http://oc.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://wm.9csxet.cn

[C16] 函数 / 方法重载
来源：http://um.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hu.lnxyls.cn

PHP:  // 无重载
来源：http://ol.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://nr.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ma.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://xe.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://mz.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ww.huanxung.cn

================================================================================
来源：http://vm.asd995.cn

D. 数组 / 列表 / 集合
来源：http://md.shtwfgs.cn

================================================================================
来源：http://pl.hahajie.cn

[D01] 创建数组 / 列表
来源：http://yr.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zd.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ma.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://id.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wl.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://br.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://qa.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://ls.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xr.9csxet.cn

[D02] 追加元素到末尾
来源：http://ey.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ls.nicolike.cn

JS:   arr.push(4);
来源：http://hd.asd995.cn

TS:   arr.push(4);
来源：http://xz.colortex.cn

Java: list.add(4);
来源：http://vf.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://eg.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://vl.shxzukj.cn

C#:   list.Add(4);
来源：http://bs.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://ch.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ag.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eu.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cb.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://ly.asd995.cn

Java: list.add(0, 0);
来源：http://de.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wi.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oq.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://hj.jctech888.com.cn

[D04] 删除元素
来源：http://go.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://st.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mm.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hq.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://ev.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ie.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nn.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zs.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bs.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://re.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fd.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rp.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://am.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://pq.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://zu.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://za.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fw.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mv.hnjuh.cn

[D06] 数组长度
来源：http://vs.colortex.cn

Py:   len(arr)
来源：http://or.colortex.cn

PHP:  count($arr);
来源：http://zi.yuexingan06.cn

JS:   arr.length
来源：http://zu.yuexingan06.cn

TS:   arr.length
来源：http://sf.jianghongdianzi.cn

Java: list.size();
来源：http://zm.nszjky.cn

Go:   len(arr)
来源：http://uz.nicolike.cn

Ruby: arr.length; arr.size
来源：http://rr.muxihuayi.cn

C#:   list.Count;
来源：http://hr.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://uw.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ab.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zg.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://lg.521024.cn

TS:   arr.slice(1, 4);
来源：http://rp.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://qh.huixiangedu.cn

Go:   arr[1:4]
来源：http://vq.lnxyls.cn

Ruby: arr[1, 3]
来源：http://vo.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ss.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://id.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://ij.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ze.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iq.muxihuayi.cn

TS:   [...a, ...b];
来源：http://mq.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dt.huanxung.cn

Go:   append(a, b...)
来源：http://mg.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://yg.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://el.9csxet.cn

[D09] 排序（升序）
来源：http://zx.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.9csxet.cn

PHP:  sort($arr);
来源：http://tp.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wz.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sy.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ih.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://do.chemitech.net.cn

Ruby: arr.sort
来源：http://eo.szsharing.cn

C#:   list.Sort();
来源：http://nd.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ke.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gg.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rg.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://di.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lc.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://so.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://af.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ya.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ve.hahajie.cn

[D11] 反转数组
来源：http://jk.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fq.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://oh.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mp.szxytkj.cn

TS:   [...arr].reverse();
来源：http://qs.newstarts.cn

Java: Collections.reverse(list);
来源：http://fz.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://ui.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ww.lnxyls.cn

C#:   list.Reverse();
来源：http://jn.haigaiapp.cn

[D12] 查找元素下标
来源：http://ok.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://do.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gp.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ey.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ax.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dn.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://qj.nicolike.cn

Ruby: arr.index(x)
来源：http://cw.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://wf.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ih.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ox.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ox.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ns.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://fa.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cb.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lz.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iw.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zq.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://eb.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ee.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tn.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://rl.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://fp.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oh.lnxyls.cn

Go:   // 手写循环
来源：http://do.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://um.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yx.newstarts.cn

[D15] 去重
来源：http://lz.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hp.gzmigu.cn

PHP:  array_unique($arr);
来源：http://vn.521024.cn

JS:   [...new Set(arr)]
来源：http://uk.nicolike.cn

TS:   [...new Set(arr)]
来源：http://kj.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jb.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yw.wgjwhj.cn

Ruby: arr.uniq
来源：http://qf.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://gy.shxzskj.cn

[D16] 求和与平均值
来源：http://ah.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mg.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hn.shxzskj.cn


<!-- 参考信息 -->