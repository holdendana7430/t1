代发 wailian999

Go:   a && b || !c
来源：http://ue.szxytkj.cn

Ruby: a && b || !c
来源：http://fl.gzmigu.cn

C#:   a && b || !c
来源：http://tx.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lx.szxytkj.cn

Py:   if not data: return
来源：http://lv.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://bd.haigaiapp.cn

JS:   if (!data) return;
来源：http://pi.colortex.cn

TS:   if (!data) return;
来源：http://sq.shxzukj.cn

Java: if (data == null) return;
来源：http://yf.haigaiapp.cn

Go:   if data == nil { return }
来源：http://hg.jctech888.com.cn

Ruby: return if data.nil?
来源：http://na.hnjuh.cn

C#:   if (data == null) return;
来源：http://xx.colortex.cn

================================================================================
来源：http://ol.huixinmuqiang.cn

C. 函数与作用域
来源：http://ex.shxzskj.cn

================================================================================
来源：http://gd.shtwfgs.cn

[C01] 定义函数
来源：http://ib.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://kt.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ui.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://hw.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ba.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rz.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lr.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://yp.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ym.newstarts.cn

[C02] 默认参数
来源：http://px.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://zb.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bt.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://qa.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jz.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kl.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tu.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://dj.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://ge.shxzukj.cn

[C03] 可变参数
来源：http://in.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://vj.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fe.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ff.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rm.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sq.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tw.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mb.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ky.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://no.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qg.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oj.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xk.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ov.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dw.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://dg.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ly.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://yk.bjjhwx.cn

[C05] 返回多个值
来源：http://ym.521024.cn

Py:   return a, b
来源：http://oe.9csxet.cn

PHP:  return [$a, $b];
来源：http://up.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ki.muxihuayi.cn

TS:   return { a, b };
来源：http://fr.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wc.jctech888.com.cn

Go:   return a, b
来源：http://gb.lnxyls.cn

Ruby: return a, b
来源：http://hr.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://pe.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://vx.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ax.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://se.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://lr.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://ca.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://de.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ly.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://td.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bh.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://hc.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kt.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kk.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pe.szsharing.cn

TS:   arr.map(String)
来源：http://eq.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ge.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wf.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://ss.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mm.huanxung.cn

[C08] 闭包
来源：http://qb.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bm.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gj.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://br.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://af.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nz.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pl.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://as.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yu.gzmigu.cn

[C09] 递归
来源：http://du.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://es.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vt.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ex.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hx.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cm.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ma.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wx.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://en.shxzukj.cn

[C10] 变量作用域
来源：http://bp.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pr.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vz.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vi.panjiajie.cn

TS:   同 JS
来源：http://ww.szxytkj.cn

Java: 方法内为块级作用域
来源：http://hv.panjiajie.cn

Go:   花括号块级作用域
来源：http://hc.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yv.colortex.cn

C#:   块级作用域
来源：http://ue.lnxyls.cn

[C11] 模块导入与导出
来源：http://ai.chemitech.net.cn

Py:   from module import func
来源：http://ws.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qj.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hk.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ph.szsharing.cn

Java: import java.util.List;
来源：http://zy.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fz.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://hr.shtwfgs.cn

C#:   using System.Text;
来源：http://nh.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://qq.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://pc.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://li.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://vh.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://jw.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mo.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://aw.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ol.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yg.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://df.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tj.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tr.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zk.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aw.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xf.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://hv.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://in.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wr.szsharing.cn

[C14] 泛型函数
来源：http://qk.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ax.chemitech.net.cn

PHP:  // 无泛型
来源：http://yj.newstarts.cn

JS:   // 无泛型
来源：http://al.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vs.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gr.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ph.lnxyls.cn

Ruby: # 无泛型
来源：http://qk.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hn.asd995.cn

[C15] 解构 / 展开参数
来源：http://ne.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yv.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://oc.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://em.jianghongdianzi.cn

Java: // 无解构
来源：http://uy.huixiangedu.cn

Go:   // 无解构
来源：http://xp.jctech888.com.cn

Ruby: a, b = pair
来源：http://nc.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://oz.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ih.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nd.nicolike.cn

PHP:  // 无重载
来源：http://zc.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lz.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://bk.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bm.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://zr.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://dv.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cb.haigaiapp.cn

================================================================================
来源：http://qu.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://th.hnjuh.cn

================================================================================
来源：http://om.9csxet.cn

[D01] 创建数组 / 列表
来源：http://by.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wr.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://du.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wc.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tu.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bt.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://ip.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://xi.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yq.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://ca.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kz.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://is.huixiangedu.cn

JS:   arr.push(4);
来源：http://up.huanxung.cn

TS:   arr.push(4);
来源：http://er.colortex.cn

Java: list.add(4);
来源：http://tf.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ho.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://ew.9csxet.cn

C#:   list.Add(4);
来源：http://ur.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://xg.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://rw.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fp.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tj.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://bx.shxzukj.cn

Java: list.add(0, 0);
来源：http://di.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uo.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mv.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://ja.lnxyls.cn

[D04] 删除元素
来源：http://rj.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cu.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cg.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cu.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://pi.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bh.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ga.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jy.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yl.lnxyls.cn

[D05] 访问与修改元素
来源：http://rb.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ve.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xq.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wa.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ic.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://yj.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://yt.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yg.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hm.nicolike.cn

[D06] 数组长度
来源：http://gp.asd995.cn

Py:   len(arr)
来源：http://dc.bjjhwx.cn

PHP:  count($arr);
来源：http://yi.huixiangedu.cn

JS:   arr.length
来源：http://gt.yuntaijiaju.cn

TS:   arr.length
来源：http://aq.yuntaijiaju.cn

Java: list.size();
来源：http://pt.yuexingan06.cn

Go:   len(arr)
来源：http://at.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://zw.yuntaijiaju.cn

C#:   list.Count;
来源：http://vo.szsharing.cn

[D07] 切片 / 取子数组
来源：http://sl.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vv.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yc.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://af.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://fo.asd995.cn

Java: list.subList(1, 4);
来源：http://hz.huixiangedu.cn

Go:   arr[1:4]
来源：http://cs.szsharing.cn

Ruby: arr[1, 3]
来源：http://ix.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://jk.9csxet.cn

[D08] 合并两个数组
来源：http://px.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://nf.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://ru.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zs.shtwfgs.cn

TS:   [...a, ...b];
来源：http://fa.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mb.haigaiapp.cn

Go:   append(a, b...)
来源：http://jp.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://yh.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://gu.bjjhwx.cn

[D09] 排序（升序）
来源：http://rd.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.nszjky.cn

PHP:  sort($arr);
来源：http://eg.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hr.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ex.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://da.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wt.bookmarksfly.cn

Ruby: arr.sort
来源：http://at.huixiangedu.cn

C#:   list.Sort();
来源：http://og.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eh.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kd.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jw.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ed.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yd.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gd.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zb.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ku.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bp.jianghongdianzi.cn

[D11] 反转数组
来源：http://bt.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bv.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ba.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ju.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://nt.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://yp.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://sh.muxihuayi.cn

Ruby: arr.reverse
来源：http://ja.bjjhwx.cn

C#:   list.Reverse();
来源：http://ec.shxzukj.cn

[D12] 查找元素下标
来源：http://uj.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://jy.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hi.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ch.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ij.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zg.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://zv.huixiangedu.cn

Ruby: arr.index(x)
来源：http://qb.asd995.cn

C#:   list.IndexOf(x);
来源：http://jv.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ri.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vb.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vc.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://sm.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://gz.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nw.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ty.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wj.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wu.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://xl.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cc.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sg.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://wu.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://ub.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oj.huixiangedu.cn

Go:   // 手写循环
来源：http://na.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ba.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ay.yuntaijiaju.cn

[D15] 去重
来源：http://zo.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tr.szxytkj.cn

PHP:  array_unique($arr);
来源：http://mj.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://nf.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://jq.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lw.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hj.9csxet.cn

Ruby: arr.uniq
来源：http://rv.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://du.muxihuayi.cn

[D16] 求和与平均值
来源：http://ev.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://az.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ay.shtwfgs.cn


<!-- 参考信息 -->