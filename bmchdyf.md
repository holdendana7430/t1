代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://xo.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://bd.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xe.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hh.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cw.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ba.521024.cn

[B15] 布尔运算与取反
来源：http://be.nicolike.cn

Py:   a and b or not c
来源：http://ag.huanxung.cn

PHP:  $a && $b || !$c
来源：http://sg.yuntaijiaju.cn

JS:   a && b || !c
来源：http://vp.wgjwhj.cn

TS:   a && b || !c
来源：http://vy.huixinmuqiang.cn

Java: a && b || !c
来源：http://yj.shxzskj.cn

Go:   a && b || !c
来源：http://bc.yuexingan06.cn

Ruby: a && b || !c
来源：http://jq.asd995.cn

C#:   a && b || !c
来源：http://vk.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xt.huixiangedu.cn

Py:   if not data: return
来源：http://ft.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://db.haigaiapp.cn

JS:   if (!data) return;
来源：http://al.shxzukj.cn

TS:   if (!data) return;
来源：http://ln.hahajie.cn

Java: if (data == null) return;
来源：http://ym.bjjhwx.cn

Go:   if data == nil { return }
来源：http://rq.yuexingan06.cn

Ruby: return if data.nil?
来源：http://oq.lnxyls.cn

C#:   if (data == null) return;
来源：http://yv.huixinmuqiang.cn

================================================================================
来源：http://hb.huanxung.cn

C. 函数与作用域
来源：http://dc.nicolike.cn

================================================================================
来源：http://gu.gzmigu.cn

[C01] 定义函数
来源：http://li.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://fu.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qp.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://jp.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gb.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dg.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pt.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://qb.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yx.szxytkj.cn

[C02] 默认参数
来源：http://ie.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://zc.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ff.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://bw.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qa.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uo.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fj.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://lu.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://pf.shxzskj.cn

[C03] 可变参数
来源：http://ml.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://zk.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jv.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xa.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yz.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vi.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gv.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ja.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jo.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://ec.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pw.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pz.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qw.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ig.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ak.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://sm.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://rr.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://fm.shxzukj.cn

[C05] 返回多个值
来源：http://kv.jianghongdianzi.cn

Py:   return a, b
来源：http://di.szxytkj.cn

PHP:  return [$a, $b];
来源：http://yb.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cl.521024.cn

TS:   return { a, b };
来源：http://hz.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uz.szxytkj.cn

Go:   return a, b
来源：http://te.huixinmuqiang.cn

Ruby: return a, b
来源：http://gq.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://bo.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://it.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://xl.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ht.szsharing.cn

JS:   const square = x => x * x;
来源：http://rf.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://yv.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ni.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lo.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://ik.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tk.asd995.cn

[C07] 把函数作为参数传入
来源：http://ss.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qg.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://co.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yg.szxytkj.cn

TS:   arr.map(String)
来源：http://ul.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ws.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gl.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ja.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gx.bookmarksfly.cn

[C08] 闭包
来源：http://nz.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rd.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ra.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bh.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mn.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mw.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jq.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zf.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uz.yuntaijiaju.cn

[C09] 递归
来源：http://ol.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pe.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kx.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fu.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zf.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ot.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xd.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ab.yuexingan06.cn

[C10] 变量作用域
来源：http://vw.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oo.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ju.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vi.bookmarksfly.cn

TS:   同 JS
来源：http://gm.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://ol.hahajie.cn

Go:   花括号块级作用域
来源：http://gy.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kv.hahajie.cn

C#:   块级作用域
来源：http://ph.shxzskj.cn

[C11] 模块导入与导出
来源：http://nh.bjjhwx.cn

Py:   from module import func
来源：http://cj.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://om.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dx.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dh.shtwfgs.cn

Java: import java.util.List;
来源：http://ao.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://li.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://pw.nicolike.cn

C#:   using System.Text;
来源：http://fr.521024.cn

[C12] 立即执行函数 IIFE
来源：http://nw.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://ep.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://wr.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://jv.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://yp.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mx.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://ho.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://fo.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nt.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://se.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jg.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jj.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xn.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wc.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://ie.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ky.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qg.jctech888.com.cn

[C14] 泛型函数
来源：http://in.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tx.chemitech.net.cn

PHP:  // 无泛型
来源：http://yd.wgjwhj.cn

JS:   // 无泛型
来源：http://dk.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yu.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://az.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ig.shtwfgs.cn

Ruby: # 无泛型
来源：http://xm.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tc.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://fr.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bg.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://bj.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fv.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sz.hahajie.cn

Java: // 无解构
来源：http://zx.haigaiapp.cn

Go:   // 无解构
来源：http://nb.gzmigu.cn

Ruby: a, b = pair
来源：http://bl.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://ax.hahajie.cn

[C16] 函数 / 方法重载
来源：http://al.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qx.yuexingan06.cn

PHP:  // 无重载
来源：http://bl.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mn.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://zx.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qs.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://yr.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://dv.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sf.wgjwhj.cn

================================================================================
来源：http://wp.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://gp.shxzukj.cn

================================================================================
来源：http://hn.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ja.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sa.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lt.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vg.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gh.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uu.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://sr.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://dq.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ad.szxytkj.cn

[D02] 追加元素到末尾
来源：http://qq.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dp.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mw.asd995.cn

JS:   arr.push(4);
来源：http://gv.nszjky.cn

TS:   arr.push(4);
来源：http://av.jctech888.com.cn

Java: list.add(4);
来源：http://vw.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://db.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://kk.shtwfgs.cn

C#:   list.Add(4);
来源：http://qj.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://rf.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://yq.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yk.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zk.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://vf.chemitech.net.cn

Java: list.add(0, 0);
来源：http://ho.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://re.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mn.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://xq.muxihuayi.cn

[D04] 删除元素
来源：http://hb.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://do.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nj.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oc.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://ko.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qz.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mh.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tr.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rc.huixiangedu.cn

[D05] 访问与修改元素
来源：http://od.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://es.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kl.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zj.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://fi.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://hk.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://bn.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mo.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://py.szsharing.cn

[D06] 数组长度
来源：http://at.shxzukj.cn

Py:   len(arr)
来源：http://rq.panjiajie.cn

PHP:  count($arr);
来源：http://gx.lnxyls.cn

JS:   arr.length
来源：http://zj.shxzukj.cn

TS:   arr.length
来源：http://gn.huanxung.cn

Java: list.size();
来源：http://jb.jianghongdianzi.cn

Go:   len(arr)
来源：http://ci.9csxet.cn

Ruby: arr.length; arr.size
来源：http://cg.huixinmuqiang.cn

C#:   list.Count;
来源：http://zn.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://xr.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pc.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vt.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://kg.asd995.cn

TS:   arr.slice(1, 4);
来源：http://bj.szsharing.cn

Java: list.subList(1, 4);
来源：http://mj.9csxet.cn

Go:   arr[1:4]
来源：http://bj.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://vn.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://vh.shxzukj.cn

[D08] 合并两个数组
来源：http://ri.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://df.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://la.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uj.newstarts.cn

TS:   [...a, ...b];
来源：http://dv.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zx.nicolike.cn

Go:   append(a, b...)
来源：http://wn.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://mz.521024.cn

C#:   a.Concat(b).ToList()
来源：http://nj.bookmarksfly.cn

[D09] 排序（升序）
来源：http://cf.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://pk.shtwfgs.cn

PHP:  sort($arr);
来源：http://vg.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zy.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wy.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ae.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rt.muxihuayi.cn

Ruby: arr.sort
来源：http://sn.muxihuayi.cn

C#:   list.Sort();
来源：http://sk.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yv.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kv.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://is.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ou.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hd.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mk.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sz.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pi.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://os.nszjky.cn

[D11] 反转数组
来源：http://iz.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://on.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://vk.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mx.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://no.lnxyls.cn

Java: Collections.reverse(list);
来源：http://tl.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://oz.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ks.szsharing.cn

C#:   list.Reverse();
来源：http://pm.yuexingan06.cn

[D12] 查找元素下标
来源：http://pi.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://ai.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wm.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kz.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qw.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jy.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://he.newstarts.cn

Ruby: arr.index(x)
来源：http://sw.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://bb.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://pn.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rf.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zg.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://hh.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://du.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nq.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kn.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pj.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mj.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://lm.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ab.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vx.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://io.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://gb.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pa.panjiajie.cn

Go:   // 手写循环
来源：http://gv.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wr.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fc.bjjhwx.cn


<!-- 参考信息 -->