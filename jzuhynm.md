代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://gv.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ro.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wj.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bu.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ri.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cy.szxytkj.cn

[B15] 布尔运算与取反
来源：http://xp.szxytkj.cn

Py:   a and b or not c
来源：http://rj.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://sr.panjiajie.cn

JS:   a && b || !c
来源：http://mh.panjiajie.cn

TS:   a && b || !c
来源：http://el.haigaiapp.cn

Java: a && b || !c
来源：http://td.huixiangedu.cn

Go:   a && b || !c
来源：http://ng.haigaiapp.cn

Ruby: a && b || !c
来源：http://oj.jctech888.com.cn

C#:   a && b || !c
来源：http://ii.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gf.nszjky.cn

Py:   if not data: return
来源：http://rr.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://ju.bookmarksfly.cn

JS:   if (!data) return;
来源：http://gw.muxihuayi.cn

TS:   if (!data) return;
来源：http://zy.jctech888.com.cn

Java: if (data == null) return;
来源：http://ef.asd995.cn

Go:   if data == nil { return }
来源：http://kx.lnxyls.cn

Ruby: return if data.nil?
来源：http://hr.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://rv.muxihuayi.cn

================================================================================
来源：http://od.9csxet.cn

C. 函数与作用域
来源：http://jg.chemitech.net.cn

================================================================================
来源：http://jv.bjjhwx.cn

[C01] 定义函数
来源：http://ek.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://id.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ya.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://zt.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oj.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gh.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uf.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://vv.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://le.521024.cn

[C02] 默认参数
来源：http://mx.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://jg.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vl.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ez.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://db.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yf.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://to.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ua.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://tn.muxihuayi.cn

[C03] 可变参数
来源：http://xm.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://jn.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://re.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://el.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tz.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jt.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cm.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ym.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ji.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ag.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hq.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bj.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ro.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vz.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://vp.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://wd.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://jq.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://vu.bjjhwx.cn

[C05] 返回多个值
来源：http://qw.jianghongdianzi.cn

Py:   return a, b
来源：http://qj.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://vp.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eq.nszjky.cn

TS:   return { a, b };
来源：http://ky.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://du.yuexingan06.cn

Go:   return a, b
来源：http://in.jctech888.com.cn

Ruby: return a, b
来源：http://ch.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://kd.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://ma.nicolike.cn

Py:   square = lambda x: x * x
来源：http://ih.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gc.nszjky.cn

JS:   const square = x => x * x;
来源：http://kp.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://my.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qe.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wh.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ox.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cq.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://tp.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xh.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rl.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vt.shxzukj.cn

TS:   arr.map(String)
来源：http://uz.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pz.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vx.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://lf.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mw.yuntaijiaju.cn

[C08] 闭包
来源：http://lu.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qj.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yg.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://va.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ix.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vq.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zb.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mk.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xp.gzmigu.cn

[C09] 递归
来源：http://av.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ee.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mz.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gt.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://up.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vk.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ls.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://of.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cd.wgjwhj.cn

[C10] 变量作用域
来源：http://ww.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qs.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://df.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mt.haigaiapp.cn

TS:   同 JS
来源：http://np.lnxyls.cn

Java: 方法内为块级作用域
来源：http://pb.chemitech.net.cn

Go:   花括号块级作用域
来源：http://qm.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iw.shtwfgs.cn

C#:   块级作用域
来源：http://hn.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ec.521024.cn

Py:   from module import func
来源：http://hd.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ow.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xc.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ec.wgjwhj.cn

Java: import java.util.List;
来源：http://wd.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pv.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://kk.chemitech.net.cn

C#:   using System.Text;
来源：http://gg.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://dg.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://uy.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ec.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://vw.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://wc.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ej.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://jc.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://gh.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zm.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://vc.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bw.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fu.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ge.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://df.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jz.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://fi.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uh.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yj.wgjwhj.cn

[C14] 泛型函数
来源：http://bi.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mx.521024.cn

PHP:  // 无泛型
来源：http://xe.nszjky.cn

JS:   // 无泛型
来源：http://dr.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ln.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ot.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://np.haigaiapp.cn

Ruby: # 无泛型
来源：http://qz.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ze.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://wb.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ve.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ov.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wu.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ap.shxzskj.cn

Java: // 无解构
来源：http://qv.521024.cn

Go:   // 无解构
来源：http://uv.wgjwhj.cn

Ruby: a, b = pair
来源：http://zg.hahajie.cn

C#:   var (a, b) = pair;
来源：http://rc.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://pb.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tn.wgjwhj.cn

PHP:  // 无重载
来源：http://kw.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ql.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://kj.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bg.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://lj.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://tr.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yp.nicolike.cn

================================================================================
来源：http://iv.colortex.cn

D. 数组 / 列表 / 集合
来源：http://he.panjiajie.cn

================================================================================
来源：http://mt.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://qi.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mi.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oa.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bl.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ur.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zc.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://eq.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://vu.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qc.gzmigu.cn

[D02] 追加元素到末尾
来源：http://lm.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uk.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wh.asd995.cn

JS:   arr.push(4);
来源：http://nh.hahajie.cn

TS:   arr.push(4);
来源：http://av.shxzskj.cn

Java: list.add(4);
来源：http://vz.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://vr.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://el.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://up.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://rd.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://dd.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fo.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ff.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://fh.yuexingan06.cn

Java: list.add(0, 0);
来源：http://nc.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jg.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jy.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://zg.hahajie.cn

[D04] 删除元素
来源：http://op.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ue.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pr.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rh.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://ty.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uz.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dx.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://le.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ho.szsharing.cn

[D05] 访问与修改元素
来源：http://aq.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nf.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ke.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://do.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://qp.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://ot.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://vl.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ce.bjjhwx.cn

[D06] 数组长度
来源：http://fl.521024.cn

Py:   len(arr)
来源：http://zt.huixiangedu.cn

PHP:  count($arr);
来源：http://vn.shxzukj.cn

JS:   arr.length
来源：http://xk.asd995.cn

TS:   arr.length
来源：http://cq.chemitech.net.cn

Java: list.size();
来源：http://dn.szsharing.cn

Go:   len(arr)
来源：http://xu.newstarts.cn

Ruby: arr.length; arr.size
来源：http://ck.jctech888.com.cn

C#:   list.Count;
来源：http://bl.hahajie.cn

[D07] 切片 / 取子数组
来源：http://wh.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gs.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gg.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://ba.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://dk.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://yi.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://lh.szxytkj.cn

Ruby: arr[1, 3]
来源：http://qg.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://og.shtwfgs.cn

[D08] 合并两个数组
来源：http://sc.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://qj.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://jr.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rh.nszjky.cn

TS:   [...a, ...b];
来源：http://ry.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zq.shtwfgs.cn

Go:   append(a, b...)
来源：http://ic.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://du.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://kc.gzmigu.cn

[D09] 排序（升序）
来源：http://zg.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ce.huanxung.cn

PHP:  sort($arr);
来源：http://cx.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pf.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fq.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mg.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nz.newstarts.cn

Ruby: arr.sort
来源：http://tp.muxihuayi.cn

C#:   list.Sort();
来源：http://xa.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yv.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lb.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ck.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xi.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qy.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vk.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oh.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qd.bjjhwx.cn

[D11] 反转数组
来源：http://uo.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sa.asd995.cn

PHP:  array_reverse($arr);
来源：http://ad.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dt.newstarts.cn

TS:   [...arr].reverse();
来源：http://ip.lnxyls.cn

Java: Collections.reverse(list);
来源：http://cy.colortex.cn

Go:   slices.Reverse(arr)
来源：http://by.hnjuh.cn

Ruby: arr.reverse
来源：http://tg.chemitech.net.cn

C#:   list.Reverse();
来源：http://pq.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://pi.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://wr.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pb.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rv.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://az.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bv.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://lb.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://oo.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://zk.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://of.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yg.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hi.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://oa.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://cx.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ll.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lx.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mf.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bg.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://lw.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hw.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://du.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://wb.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://qe.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ks.shtwfgs.cn

Go:   // 手写循环
来源：http://ng.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ld.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kp.nicolike.cn


<!-- 参考信息 -->