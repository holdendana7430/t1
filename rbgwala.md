代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://uf.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yr.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ot.gzmigu.cn

Py:   a and b or not c
来源：http://hu.szsharing.cn

PHP:  $a && $b || !$c
来源：http://tf.gzmigu.cn

JS:   a && b || !c
来源：http://uk.panjiajie.cn

TS:   a && b || !c
来源：http://zi.chemitech.net.cn

Java: a && b || !c
来源：http://ix.521024.cn

Go:   a && b || !c
来源：http://rv.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://rc.newstarts.cn

C#:   a && b || !c
来源：http://ct.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nl.newstarts.cn

Py:   if not data: return
来源：http://so.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://gn.lnxyls.cn

JS:   if (!data) return;
来源：http://sk.muxihuayi.cn

TS:   if (!data) return;
来源：http://rf.newstarts.cn

Java: if (data == null) return;
来源：http://gt.colortex.cn

Go:   if data == nil { return }
来源：http://lo.bjjhwx.cn

Ruby: return if data.nil?
来源：http://sb.szsharing.cn

C#:   if (data == null) return;
来源：http://kd.newstarts.cn

================================================================================
来源：http://wy.9csxet.cn

C. 函数与作用域
来源：http://da.shtwfgs.cn

================================================================================
来源：http://bf.hnjuh.cn

[C01] 定义函数
来源：http://iz.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://uv.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lz.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://oz.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xj.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ae.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qd.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://fg.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ur.newstarts.cn

[C02] 默认参数
来源：http://xb.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://yu.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nx.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://zv.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bl.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ct.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uy.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://xx.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://ga.panjiajie.cn

[C03] 可变参数
来源：http://yd.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://zu.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tu.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fh.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tg.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xk.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rb.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cq.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://al.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://kl.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cw.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hc.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oy.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cp.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://nh.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://eb.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://td.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://bq.jianghongdianzi.cn

[C05] 返回多个值
来源：http://jj.hahajie.cn

Py:   return a, b
来源：http://un.szsharing.cn

PHP:  return [$a, $b];
来源：http://ox.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zg.szxytkj.cn

TS:   return { a, b };
来源：http://ti.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zc.wgjwhj.cn

Go:   return a, b
来源：http://tw.panjiajie.cn

Ruby: return a, b
来源：http://ep.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://zl.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ql.colortex.cn

Py:   square = lambda x: x * x
来源：http://ym.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ek.9csxet.cn

JS:   const square = x => x * x;
来源：http://mk.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://yd.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fd.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dx.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://yr.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mn.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ib.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pa.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kh.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tr.panjiajie.cn

TS:   arr.map(String)
来源：http://fa.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ln.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://by.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://ca.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sv.shtwfgs.cn

[C08] 闭包
来源：http://pz.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bt.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oy.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mk.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lx.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://az.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dx.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jq.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lw.wgjwhj.cn

[C09] 递归
来源：http://lz.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ds.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oe.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ad.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://if.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mn.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://da.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kf.yuexingan06.cn

[C10] 变量作用域
来源：http://gk.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://km.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zc.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kv.521024.cn

TS:   同 JS
来源：http://hf.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://ij.haigaiapp.cn

Go:   花括号块级作用域
来源：http://jq.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ip.hahajie.cn

C#:   块级作用域
来源：http://ig.colortex.cn

[C11] 模块导入与导出
来源：http://jo.lnxyls.cn

Py:   from module import func
来源：http://cy.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hf.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gp.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kq.shxzukj.cn

Java: import java.util.List;
来源：http://ef.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://py.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://mq.huanxung.cn

C#:   using System.Text;
来源：http://pe.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://qh.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://us.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://rb.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ht.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://jj.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://in.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pn.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://qi.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pt.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://ny.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hr.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wu.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nu.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jf.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vo.panjiajie.cn

Go:   func add(a, b int) int
来源：http://il.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ns.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://us.huixiangedu.cn

[C14] 泛型函数
来源：http://sv.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xm.gzmigu.cn

PHP:  // 无泛型
来源：http://up.haigaiapp.cn

JS:   // 无泛型
来源：http://pe.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wd.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nr.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ga.szsharing.cn

Ruby: # 无泛型
来源：http://hk.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yb.huanxung.cn

[C15] 解构 / 展开参数
来源：http://jn.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ql.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://kx.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://is.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bh.chemitech.net.cn

Java: // 无解构
来源：http://cn.yuntaijiaju.cn

Go:   // 无解构
来源：http://iq.szsharing.cn

Ruby: a, b = pair
来源：http://ut.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://nu.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://pg.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yl.jctech888.com.cn

PHP:  // 无重载
来源：http://dg.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zs.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://by.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cm.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://sl.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://na.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bq.nicolike.cn

================================================================================
来源：http://tl.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://rs.szsharing.cn

================================================================================
来源：http://wj.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://tt.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vc.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qf.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oz.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ph.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ih.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://uo.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://fz.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pd.9csxet.cn

[D02] 追加元素到末尾
来源：http://jr.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wh.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hh.521024.cn

JS:   arr.push(4);
来源：http://wl.wgjwhj.cn

TS:   arr.push(4);
来源：http://he.newstarts.cn

Java: list.add(4);
来源：http://tt.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://hm.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://jc.szxytkj.cn

C#:   list.Add(4);
来源：http://xj.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://vi.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://ah.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kk.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dr.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://px.colortex.cn

Java: list.add(0, 0);
来源：http://oh.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dn.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://th.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://yl.huixiangedu.cn

[D04] 删除元素
来源：http://og.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oo.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pn.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nl.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://ae.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dw.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qb.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qe.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vl.hnjuh.cn

[D05] 访问与修改元素
来源：http://sj.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://no.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pd.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pb.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://wk.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://hi.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://uj.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pv.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dy.yuexingan06.cn

[D06] 数组长度
来源：http://by.haigaiapp.cn

Py:   len(arr)
来源：http://xv.wgjwhj.cn

PHP:  count($arr);
来源：http://dc.gzmigu.cn

JS:   arr.length
来源：http://cz.wgjwhj.cn

TS:   arr.length
来源：http://kl.szsharing.cn

Java: list.size();
来源：http://zc.jctech888.com.cn

Go:   len(arr)
来源：http://wz.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://hi.szxytkj.cn

C#:   list.Count;
来源：http://sm.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ib.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yu.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fm.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://gq.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://wm.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://mg.asd995.cn

Go:   arr[1:4]
来源：http://pg.newstarts.cn

Ruby: arr[1, 3]
来源：http://xd.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://yy.szxytkj.cn

[D08] 合并两个数组
来源：http://iq.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://xc.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://po.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kb.jctech888.com.cn

TS:   [...a, ...b];
来源：http://vj.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dd.haigaiapp.cn

Go:   append(a, b...)
来源：http://ul.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://wx.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://wm.jctech888.com.cn

[D09] 排序（升序）
来源：http://ka.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qj.521024.cn

PHP:  sort($arr);
来源：http://bw.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dw.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gh.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zr.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wy.huixiangedu.cn

Ruby: arr.sort
来源：http://jg.shxzskj.cn

C#:   list.Sort();
来源：http://ke.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hn.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qj.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://he.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tx.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kj.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xv.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ps.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cu.shxzskj.cn

[D11] 反转数组
来源：http://lz.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ns.nicolike.cn

PHP:  array_reverse($arr);
来源：http://kn.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pk.szsharing.cn

TS:   [...arr].reverse();
来源：http://fk.newstarts.cn

Java: Collections.reverse(list);
来源：http://ky.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://no.szsharing.cn

Ruby: arr.reverse
来源：http://nv.lnxyls.cn

C#:   list.Reverse();
来源：http://dq.huixiangedu.cn

[D12] 查找元素下标
来源：http://tv.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://ms.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xb.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zx.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mx.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://oo.colortex.cn

Ruby: arr.index(x)
来源：http://ti.521024.cn

C#:   list.IndexOf(x);
来源：http://mx.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://jc.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jm.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tx.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://dh.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://jj.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qq.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://io.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qf.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jj.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://nb.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uz.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vj.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://wc.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://so.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xk.jctech888.com.cn

Go:   // 手写循环
来源：http://zb.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tq.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xp.hahajie.cn

[D15] 去重
来源：http://mu.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jx.hnjuh.cn

PHP:  array_unique($arr);
来源：http://is.szsharing.cn

JS:   [...new Set(arr)]
来源：http://ip.huixiangedu.cn


<!-- 参考信息 -->