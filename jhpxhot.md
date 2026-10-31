代发 wailian999

[B13] 判断是否为数字
来源：http://qm.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://mk.shxzukj.cn

PHP:  is_numeric($x)
来源：http://cd.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://es.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://af.jctech888.com.cn

Java: x instanceof Number
来源：http://kn.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gu.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://yz.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://ay.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://ma.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vz.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dz.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://og.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://ak.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vj.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fg.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ug.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://no.szxytkj.cn

[B15] 布尔运算与取反
来源：http://gt.gzmigu.cn

Py:   a and b or not c
来源：http://oz.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://op.huixiangedu.cn

JS:   a && b || !c
来源：http://mf.hahajie.cn

TS:   a && b || !c
来源：http://bh.haigaiapp.cn

Java: a && b || !c
来源：http://qp.shxzskj.cn

Go:   a && b || !c
来源：http://lz.shxzskj.cn

Ruby: a && b || !c
来源：http://ow.colortex.cn

C#:   a && b || !c
来源：http://jo.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zt.colortex.cn

Py:   if not data: return
来源：http://nr.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://fp.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://fk.nszjky.cn

TS:   if (!data) return;
来源：http://xh.yuexingan06.cn

Java: if (data == null) return;
来源：http://wr.nszjky.cn

Go:   if data == nil { return }
来源：http://cu.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://wc.yuexingan06.cn

C#:   if (data == null) return;
来源：http://mm.gzmigu.cn

================================================================================
来源：http://ig.haigaiapp.cn

C. 函数与作用域
来源：http://cs.muxihuayi.cn

================================================================================
来源：http://hf.gzmigu.cn

[C01] 定义函数
来源：http://bo.asd995.cn

Py:   def add(a, b): return a + b
来源：http://fb.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://le.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://io.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wd.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ge.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nk.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://kt.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tj.haigaiapp.cn

[C02] 默认参数
来源：http://go.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ir.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pj.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hv.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gf.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gs.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pv.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://xs.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://mo.szsharing.cn

[C03] 可变参数
来源：http://uh.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ml.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uv.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jm.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ki.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ye.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wr.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xq.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://tn.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://em.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eb.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uq.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qx.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://fg.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://id.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://pv.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://ly.huanxung.cn

[C05] 返回多个值
来源：http://uk.szxytkj.cn

Py:   return a, b
来源：http://yb.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://rg.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lq.jctech888.com.cn

TS:   return { a, b };
来源：http://xt.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://py.jctech888.com.cn

Go:   return a, b
来源：http://va.asd995.cn

Ruby: return a, b
来源：http://my.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ob.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://wn.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://tf.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zl.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://hb.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://gk.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ku.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ge.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://vj.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jo.521024.cn

[C07] 把函数作为参数传入
来源：http://qq.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xn.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ym.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cr.huixiangedu.cn

TS:   arr.map(String)
来源：http://xt.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ji.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pz.521024.cn

Ruby: arr.map(&:upcase)
来源：http://me.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://le.huixiangedu.cn

[C08] 闭包
来源：http://fm.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://re.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xz.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qf.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://na.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vg.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://on.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ts.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lw.asd995.cn

[C09] 递归
来源：http://ff.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xv.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qt.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ut.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bl.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ko.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://np.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gb.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lu.chemitech.net.cn

[C10] 变量作用域
来源：http://yp.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mz.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lw.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pk.huixinmuqiang.cn

TS:   同 JS
来源：http://iy.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://tb.asd995.cn

Go:   花括号块级作用域
来源：http://zm.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://th.colortex.cn

C#:   块级作用域
来源：http://gh.szsharing.cn

[C11] 模块导入与导出
来源：http://en.yuexingan06.cn

Py:   from module import func
来源：http://xq.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eu.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ln.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hc.9csxet.cn

Java: import java.util.List;
来源：http://yi.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qo.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.9csxet.cn

C#:   using System.Text;
来源：http://sb.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ii.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://gw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://al.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ec.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://qd.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lu.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ij.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://uu.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ld.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://ny.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://de.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://od.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wa.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://po.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://da.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://pi.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ff.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xk.jianghongdianzi.cn

[C14] 泛型函数
来源：http://iv.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://da.bjjhwx.cn

PHP:  // 无泛型
来源：http://sx.9csxet.cn

JS:   // 无泛型
来源：http://vn.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ce.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hc.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ft.szxytkj.cn

Ruby: # 无泛型
来源：http://xt.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ze.huanxung.cn

[C15] 解构 / 展开参数
来源：http://pm.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ti.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://zh.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iy.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gl.yuexingan06.cn

Java: // 无解构
来源：http://ap.bjjhwx.cn

Go:   // 无解构
来源：http://wp.szsharing.cn

Ruby: a, b = pair
来源：http://cd.asd995.cn

C#:   var (a, b) = pair;
来源：http://ut.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://nn.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dp.hnjuh.cn

PHP:  // 无重载
来源：http://nk.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ep.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://tq.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dr.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ow.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://cf.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://un.nicolike.cn

================================================================================
来源：http://ij.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://lx.colortex.cn

================================================================================
来源：http://vk.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://zj.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rv.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://en.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ws.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wy.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bx.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://zw.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://pf.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nq.hahajie.cn

[D02] 追加元素到末尾
来源：http://ue.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kh.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qc.szxytkj.cn

JS:   arr.push(4);
来源：http://ny.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://wd.nszjky.cn

Java: list.add(4);
来源：http://ts.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://cc.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ik.521024.cn

C#:   list.Add(4);
来源：http://ve.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://vq.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://df.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dm.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jn.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://nz.muxihuayi.cn

Java: list.add(0, 0);
来源：http://ai.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dc.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://uo.jianghongdianzi.cn

[D04] 删除元素
来源：http://yx.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pa.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iv.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ts.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://po.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bx.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ip.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bg.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aj.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://gx.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yh.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nx.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ig.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://ya.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://lq.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vk.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ic.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jd.szsharing.cn

[D06] 数组长度
来源：http://uc.nicolike.cn

Py:   len(arr)
来源：http://dt.wgjwhj.cn

PHP:  count($arr);
来源：http://if.hnjuh.cn

JS:   arr.length
来源：http://wg.gzmigu.cn

TS:   arr.length
来源：http://qi.lnxyls.cn

Java: list.size();
来源：http://fb.huixinmuqiang.cn

Go:   len(arr)
来源：http://fu.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://af.yuexingan06.cn

C#:   list.Count;
来源：http://kl.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://hc.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xw.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://je.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://aq.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://or.szxytkj.cn

Java: list.subList(1, 4);
来源：http://td.colortex.cn

Go:   arr[1:4]
来源：http://wj.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://ya.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://do.haigaiapp.cn

[D08] 合并两个数组
来源：http://db.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://lt.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://dl.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ew.nszjky.cn

TS:   [...a, ...b];
来源：http://kw.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iy.jctech888.com.cn

Go:   append(a, b...)
来源：http://bu.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://pk.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://kk.9csxet.cn

[D09] 排序（升序）
来源：http://hm.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://za.nszjky.cn

PHP:  sort($arr);
来源：http://xt.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yg.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xa.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wv.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://et.huanxung.cn

Ruby: arr.sort
来源：http://hj.muxihuayi.cn

C#:   list.Sort();
来源：http://kv.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cp.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ko.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://be.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sa.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pr.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cs.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wu.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ok.huixinmuqiang.cn

[D11] 反转数组
来源：http://mk.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://on.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://uo.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vr.shxzskj.cn

TS:   [...arr].reverse();
来源：http://px.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://ot.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://wo.lnxyls.cn

Ruby: arr.reverse
来源：http://qy.yuexingan06.cn

C#:   list.Reverse();
来源：http://ap.521024.cn

[D12] 查找元素下标
来源：http://jd.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://rx.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qg.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uz.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gn.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rc.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://bh.hnjuh.cn

Ruby: arr.index(x)
来源：http://ad.521024.cn

C#:   list.IndexOf(x);
来源：http://fd.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://lb.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dg.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gz.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://gx.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://wx.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zm.hnjuh.cn


<!-- 参考信息 -->