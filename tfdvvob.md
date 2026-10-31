代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nl.yuexingan06.cn

Java: x instanceof Number
来源：http://ki.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vy.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://xg.lnxyls.cn

C#:   x is int or double or decimal
来源：http://yk.asd995.cn

[B14] 判断值是否在集合内
来源：http://rx.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bu.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rh.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://rb.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://px.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vz.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pz.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ft.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ak.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://vr.muxihuayi.cn

Py:   a and b or not c
来源：http://vp.asd995.cn

PHP:  $a && $b || !$c
来源：http://pg.bookmarksfly.cn

JS:   a && b || !c
来源：http://ox.shtwfgs.cn

TS:   a && b || !c
来源：http://gl.521024.cn

Java: a && b || !c
来源：http://qu.huixiangedu.cn

Go:   a && b || !c
来源：http://qi.shxzukj.cn

Ruby: a && b || !c
来源：http://ce.gzmigu.cn

C#:   a && b || !c
来源：http://qv.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mm.jianghongdianzi.cn

Py:   if not data: return
来源：http://px.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://tx.huixiangedu.cn

JS:   if (!data) return;
来源：http://ni.haigaiapp.cn

TS:   if (!data) return;
来源：http://va.yuexingan06.cn

Java: if (data == null) return;
来源：http://ti.nszjky.cn

Go:   if data == nil { return }
来源：http://qx.haigaiapp.cn

Ruby: return if data.nil?
来源：http://iy.nicolike.cn

C#:   if (data == null) return;
来源：http://yk.yuntaijiaju.cn

================================================================================
来源：http://cy.nicolike.cn

C. 函数与作用域
来源：http://zl.wgjwhj.cn

================================================================================
来源：http://iz.szxytkj.cn

[C01] 定义函数
来源：http://op.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://yw.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aw.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://os.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ct.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://io.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xh.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://wd.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qx.muxihuayi.cn

[C02] 默认参数
来源：http://qv.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://es.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yh.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://fu.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://in.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dl.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nr.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://ae.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://dk.jctech888.com.cn

[C03] 可变参数
来源：http://sq.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ix.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ms.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ng.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://us.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wo.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wr.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lh.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qw.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://bj.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fd.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iw.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gn.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ay.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://ox.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://tw.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://rh.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://oh.huixiangedu.cn

[C05] 返回多个值
来源：http://xw.521024.cn

Py:   return a, b
来源：http://ku.asd995.cn

PHP:  return [$a, $b];
来源：http://hv.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ee.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ur.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xt.bjjhwx.cn

Go:   return a, b
来源：http://ai.hahajie.cn

Ruby: return a, b
来源：http://bg.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://mn.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://yw.szsharing.cn

Py:   square = lambda x: x * x
来源：http://xq.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dm.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://qe.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://hq.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lt.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ss.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://gl.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xa.9csxet.cn

[C07] 把函数作为参数传入
来源：http://ad.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aj.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ph.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://je.hahajie.cn

TS:   arr.map(String)
来源：http://ib.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://en.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ul.521024.cn

Ruby: arr.map(&:upcase)
来源：http://zo.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://na.shxzukj.cn

[C08] 闭包
来源：http://nl.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eo.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hv.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ew.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ub.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mm.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zm.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://em.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vd.wgjwhj.cn

[C09] 递归
来源：http://qk.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ob.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bo.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cw.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wz.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ps.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cg.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aq.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://un.nszjky.cn

[C10] 变量作用域
来源：http://nq.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kg.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gr.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qu.bjjhwx.cn

TS:   同 JS
来源：http://vv.szxytkj.cn

Java: 方法内为块级作用域
来源：http://rz.wgjwhj.cn

Go:   花括号块级作用域
来源：http://uz.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.shxzukj.cn

C#:   块级作用域
来源：http://yr.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://aw.szsharing.cn

Py:   from module import func
来源：http://cz.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tv.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ii.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://id.asd995.cn

Java: import java.util.List;
来源：http://rx.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zf.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://bx.haigaiapp.cn

C#:   using System.Text;
来源：http://fn.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://kp.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://mq.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://kx.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://sw.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://gf.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sq.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://kp.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ep.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uc.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ws.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fi.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qx.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dm.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ow.szsharing.cn

Go:   func add(a, b int) int
来源：http://ka.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wl.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fg.szxytkj.cn

[C14] 泛型函数
来源：http://ad.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ha.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://lm.huixinmuqiang.cn

JS:   // 无泛型
来源：http://oz.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://is.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qe.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hw.huanxung.cn

Ruby: # 无泛型
来源：http://yu.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://it.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://hr.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mt.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://be.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lb.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://um.hahajie.cn

Java: // 无解构
来源：http://vk.nszjky.cn

Go:   // 无解构
来源：http://dc.yuexingan06.cn

Ruby: a, b = pair
来源：http://mi.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://qs.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://ug.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wj.huixinmuqiang.cn

PHP:  // 无重载
来源：http://vv.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kv.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://xg.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pg.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://lj.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://rn.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://se.hnjuh.cn

================================================================================
来源：http://fr.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://jd.nszjky.cn

================================================================================
来源：http://it.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://xt.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bm.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fk.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tf.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://be.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://at.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://pu.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://id.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pw.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://ur.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bn.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sj.asd995.cn

JS:   arr.push(4);
来源：http://np.jctech888.com.cn

TS:   arr.push(4);
来源：http://yk.bjjhwx.cn

Java: list.add(4);
来源：http://nn.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://oh.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://pw.521024.cn

C#:   list.Add(4);
来源：http://kt.9csxet.cn

[D03] 在指定位置插入元素
来源：http://zt.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://qz.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ud.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://do.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://eq.521024.cn

Java: list.add(0, 0);
来源：http://tf.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jc.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tn.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://wb.hnjuh.cn

[D04] 删除元素
来源：http://zi.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aq.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jg.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qv.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://vb.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wj.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fa.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dn.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zd.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://tg.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://as.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ql.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://og.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://il.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://kc.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://yf.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rl.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dr.yuntaijiaju.cn

[D06] 数组长度
来源：http://ie.panjiajie.cn

Py:   len(arr)
来源：http://eo.shxzskj.cn

PHP:  count($arr);
来源：http://vv.bookmarksfly.cn

JS:   arr.length
来源：http://gp.jctech888.com.cn

TS:   arr.length
来源：http://hu.huixiangedu.cn

Java: list.size();
来源：http://ia.hahajie.cn

Go:   len(arr)
来源：http://kd.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://wl.gzmigu.cn

C#:   list.Count;
来源：http://sy.hahajie.cn

[D07] 切片 / 取子数组
来源：http://bz.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kh.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qw.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://by.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://jg.hnjuh.cn

Java: list.subList(1, 4);
来源：http://gg.nicolike.cn

Go:   arr[1:4]
来源：http://aj.nszjky.cn

Ruby: arr[1, 3]
来源：http://li.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://ju.gzmigu.cn

[D08] 合并两个数组
来源：http://qe.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://vu.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://rs.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ij.521024.cn

TS:   [...a, ...b];
来源：http://pa.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kf.521024.cn

Go:   append(a, b...)
来源：http://iq.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://so.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://lk.hahajie.cn

[D09] 排序（升序）
来源：http://cx.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wt.wgjwhj.cn

PHP:  sort($arr);
来源：http://ll.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ng.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cv.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ej.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tv.haigaiapp.cn

Ruby: arr.sort
来源：http://mp.hnjuh.cn

C#:   list.Sort();
来源：http://rh.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dk.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rt.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iu.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://at.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://px.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ey.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jx.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ya.huanxung.cn

[D11] 反转数组
来源：http://ja.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mg.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://jz.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dx.shxzukj.cn

TS:   [...arr].reverse();
来源：http://xb.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://lt.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://lz.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ae.gzmigu.cn

C#:   list.Reverse();
来源：http://xw.jctech888.com.cn

[D12] 查找元素下标
来源：http://rs.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://yk.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wd.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://li.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://po.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gj.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://yj.nicolike.cn

Ruby: arr.index(x)
来源：http://bs.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://qr.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://hb.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oo.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dx.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://xc.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://vt.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ss.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ca.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qx.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ds.huixinmuqiang.cn


<!-- 参考信息 -->