代发 wailian999

Go:   a && b || !c
来源：http://sx.shxzskj.cn

Ruby: a && b || !c
来源：http://oo.szsharing.cn

C#:   a && b || !c
来源：http://ur.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vx.szxytkj.cn

Py:   if not data: return
来源：http://lv.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://tz.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://is.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://ol.9csxet.cn

Java: if (data == null) return;
来源：http://bw.9csxet.cn

Go:   if data == nil { return }
来源：http://um.szsharing.cn

Ruby: return if data.nil?
来源：http://rz.chemitech.net.cn

C#:   if (data == null) return;
来源：http://bj.yuntaijiaju.cn

================================================================================
来源：http://mn.yuntaijiaju.cn

C. 函数与作用域
来源：http://om.asd995.cn

================================================================================
来源：http://kw.hnjuh.cn

[C01] 定义函数
来源：http://zc.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://bv.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mx.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://pi.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bt.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hf.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dx.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://wv.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vw.jianghongdianzi.cn

[C02] 默认参数
来源：http://ei.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://db.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ya.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://lz.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nk.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oi.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://te.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nj.521024.cn

[C03] 可变参数
来源：http://vs.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://zy.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ns.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vk.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xa.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jk.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xw.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zz.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://iy.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zf.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ln.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ix.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uo.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://tn.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://nv.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://tq.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://mi.hahajie.cn

[C05] 返回多个值
来源：http://pl.nicolike.cn

Py:   return a, b
来源：http://hs.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ty.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yx.yuexingan06.cn

TS:   return { a, b };
来源：http://kd.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yq.jianghongdianzi.cn

Go:   return a, b
来源：http://gl.shxzukj.cn

Ruby: return a, b
来源：http://ma.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://oc.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://mj.9csxet.cn

Py:   square = lambda x: x * x
来源：http://nd.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ew.hnjuh.cn

JS:   const square = x => x * x;
来源：http://wi.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ha.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bo.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ma.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://hq.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://no.newstarts.cn

[C07] 把函数作为参数传入
来源：http://sr.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pk.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dc.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wa.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://vj.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xg.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jk.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://mq.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jo.yuntaijiaju.cn

[C08] 闭包
来源：http://sv.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ag.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qb.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ye.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fh.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zp.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vp.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zv.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kl.panjiajie.cn

[C09] 递归
来源：http://dv.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mv.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ad.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://px.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xn.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jj.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fx.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yw.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iu.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ru.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ph.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jm.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tb.asd995.cn

TS:   同 JS
来源：http://ab.panjiajie.cn

Java: 方法内为块级作用域
来源：http://xh.panjiajie.cn

Go:   花括号块级作用域
来源：http://ux.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uy.nicolike.cn

C#:   块级作用域
来源：http://xw.newstarts.cn

[C11] 模块导入与导出
来源：http://wz.9csxet.cn

Py:   from module import func
来源：http://zj.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xb.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vo.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oa.bjjhwx.cn

Java: import java.util.List;
来源：http://gq.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iy.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://xc.newstarts.cn

C#:   using System.Text;
来源：http://be.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://em.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://bw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://vm.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ih.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://lo.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://km.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://mw.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://uh.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ob.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://lb.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ds.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fs.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sh.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rw.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ns.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nd.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lh.muxihuayi.cn

[C14] 泛型函数
来源：http://sf.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yh.yuexingan06.cn

PHP:  // 无泛型
来源：http://ox.jctech888.com.cn

JS:   // 无泛型
来源：http://qf.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pg.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sr.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eo.wgjwhj.cn

Ruby: # 无泛型
来源：http://pj.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wg.newstarts.cn

[C15] 解构 / 展开参数
来源：http://fu.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://us.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://kb.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qf.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ff.asd995.cn

Java: // 无解构
来源：http://bk.muxihuayi.cn

Go:   // 无解构
来源：http://fs.szsharing.cn

Ruby: a, b = pair
来源：http://lo.colortex.cn

C#:   var (a, b) = pair;
来源：http://rs.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://if.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yo.haigaiapp.cn

PHP:  // 无重载
来源：http://iz.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://du.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://ur.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zv.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://te.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://di.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jg.bjjhwx.cn

================================================================================
来源：http://hb.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://na.huanxung.cn

================================================================================
来源：http://iz.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://mb.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bx.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gb.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vr.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://je.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jh.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://os.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://vd.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://az.shxzukj.cn

[D02] 追加元素到末尾
来源：http://rw.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gk.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://of.bjjhwx.cn

JS:   arr.push(4);
来源：http://nw.hnjuh.cn

TS:   arr.push(4);
来源：http://gx.jianghongdianzi.cn

Java: list.add(4);
来源：http://vn.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://wv.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://eu.wgjwhj.cn

C#:   list.Add(4);
来源：http://da.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://yw.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ux.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gj.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uf.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://gr.haigaiapp.cn

Java: list.add(0, 0);
来源：http://hn.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ys.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://en.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://wj.lnxyls.cn

[D04] 删除元素
来源：http://sg.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fd.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uv.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fd.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://vq.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uk.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xm.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ut.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kv.newstarts.cn

[D05] 访问与修改元素
来源：http://dq.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://js.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mt.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://za.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://zp.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://er.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://gh.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://an.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ph.bookmarksfly.cn

[D06] 数组长度
来源：http://ns.haigaiapp.cn

Py:   len(arr)
来源：http://gj.huanxung.cn

PHP:  count($arr);
来源：http://al.bjjhwx.cn

JS:   arr.length
来源：http://rh.bjjhwx.cn

TS:   arr.length
来源：http://mf.shtwfgs.cn

Java: list.size();
来源：http://yp.szxytkj.cn

Go:   len(arr)
来源：http://gh.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://aw.hahajie.cn

C#:   list.Count;
来源：http://ox.szsharing.cn

[D07] 切片 / 取子数组
来源：http://le.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ao.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ff.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://oo.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://av.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://sa.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://qt.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://ux.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://wv.szxytkj.cn

[D08] 合并两个数组
来源：http://hl.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ju.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://qp.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zv.newstarts.cn

TS:   [...a, ...b];
来源：http://jm.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rd.szsharing.cn

Go:   append(a, b...)
来源：http://yt.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://pt.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://la.panjiajie.cn

[D09] 排序（升序）
来源：http://ce.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://gj.shtwfgs.cn

PHP:  sort($arr);
来源：http://nf.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ln.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zr.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ly.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mo.jianghongdianzi.cn

Ruby: arr.sort
来源：http://fd.nicolike.cn

C#:   list.Sort();
来源：http://nq.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jm.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ae.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cz.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tp.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bn.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lb.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tu.nszjky.cn

[D11] 反转数组
来源：http://ya.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ei.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://ic.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nr.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://yc.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://hm.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://so.hnjuh.cn

Ruby: arr.reverse
来源：http://ey.nicolike.cn

C#:   list.Reverse();
来源：http://gy.hahajie.cn

[D12] 查找元素下标
来源：http://kn.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://zx.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tb.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ab.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yd.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://br.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://qt.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://fx.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://dy.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fk.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ed.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://lw.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://bw.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ho.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fz.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tp.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lu.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://gg.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sd.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tj.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://tc.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://kf.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bz.jianghongdianzi.cn

Go:   // 手写循环
来源：http://pr.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ho.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hk.haigaiapp.cn

[D15] 去重
来源：http://en.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ns.newstarts.cn

PHP:  array_unique($arr);
来源：http://py.521024.cn

JS:   [...new Set(arr)]
来源：http://nh.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://vh.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rk.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://am.521024.cn

Ruby: arr.uniq
来源：http://jt.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://ct.gzmigu.cn

[D16] 求和与平均值
来源：http://md.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fh.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ka.asd995.cn


<!-- 参考信息 -->