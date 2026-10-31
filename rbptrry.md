代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ko.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://sw.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oe.shxzskj.cn

[B12] 跳出多层循环
来源：http://jt.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kd.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mf.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ba.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tu.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sq.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zd.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fe.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cq.shxzukj.cn

[B13] 判断是否为数字
来源：http://iz.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ij.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://rb.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ru.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xv.wgjwhj.cn

Java: x instanceof Number
来源：http://xa.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fu.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://gv.panjiajie.cn

C#:   x is int or double or decimal
来源：http://cy.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://fe.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ge.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vw.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://aj.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://tt.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ms.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ee.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cz.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eu.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://wv.panjiajie.cn

Py:   a and b or not c
来源：http://nh.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://uo.huixiangedu.cn

JS:   a && b || !c
来源：http://yv.chemitech.net.cn

TS:   a && b || !c
来源：http://bt.huixiangedu.cn

Java: a && b || !c
来源：http://am.shxzskj.cn

Go:   a && b || !c
来源：http://tj.panjiajie.cn

Ruby: a && b || !c
来源：http://rl.gzmigu.cn

C#:   a && b || !c
来源：http://lz.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tg.nicolike.cn

Py:   if not data: return
来源：http://gs.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://cs.gzmigu.cn

JS:   if (!data) return;
来源：http://hq.hnjuh.cn

TS:   if (!data) return;
来源：http://cl.chemitech.net.cn

Java: if (data == null) return;
来源：http://tb.hahajie.cn

Go:   if data == nil { return }
来源：http://rn.shxzukj.cn

Ruby: return if data.nil?
来源：http://if.huanxung.cn

C#:   if (data == null) return;
来源：http://at.huanxung.cn

================================================================================
来源：http://dv.asd995.cn

C. 函数与作用域
来源：http://ht.shxzukj.cn

================================================================================
来源：http://ru.shxzukj.cn

[C01] 定义函数
来源：http://mk.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://rx.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zm.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://of.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hn.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zk.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vs.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://bo.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rs.panjiajie.cn

[C02] 默认参数
来源：http://tu.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://es.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wg.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tu.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ut.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qm.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vn.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://ik.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://qz.huixiangedu.cn

[C03] 可变参数
来源：http://cb.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://qu.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vr.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://we.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ij.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nf.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://up.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ny.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://zc.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sj.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ov.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ln.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ds.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://pj.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://ij.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://wb.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://gw.asd995.cn

[C05] 返回多个值
来源：http://wj.yuntaijiaju.cn

Py:   return a, b
来源：http://nw.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://tk.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mj.panjiajie.cn

TS:   return { a, b };
来源：http://zl.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hx.nicolike.cn

Go:   return a, b
来源：http://mu.huixinmuqiang.cn

Ruby: return a, b
来源：http://nh.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://rc.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://dk.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://io.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kf.szxytkj.cn

JS:   const square = x => x * x;
来源：http://dx.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://dn.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ik.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://as.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://du.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vd.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sk.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ap.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://cr.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bs.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mq.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ua.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pu.wgjwhj.cn

[C08] 闭包
来源：http://rr.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fe.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yu.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yu.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bg.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xk.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cz.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rx.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fl.jianghongdianzi.cn

[C09] 递归
来源：http://lg.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gz.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nx.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hk.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lh.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gw.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vz.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pn.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ai.huixinmuqiang.cn

[C10] 变量作用域
来源：http://kz.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ff.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dv.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xf.panjiajie.cn

TS:   同 JS
来源：http://bk.huanxung.cn

Java: 方法内为块级作用域
来源：http://kd.huixiangedu.cn

Go:   花括号块级作用域
来源：http://lj.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ae.shxzukj.cn

C#:   块级作用域
来源：http://ka.shxzskj.cn

[C11] 模块导入与导出
来源：http://xj.nszjky.cn

Py:   from module import func
来源：http://lo.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vu.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tz.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lu.yuntaijiaju.cn

Java: import java.util.List;
来源：http://hl.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://be.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://oz.yuexingan06.cn

C#:   using System.Text;
来源：http://kk.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://sd.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://hi.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://re.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://my.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://pa.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ow.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://wl.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://zm.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yp.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://fn.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hx.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vv.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dr.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hf.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://id.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://pd.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nm.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eu.shxzukj.cn

[C14] 泛型函数
来源：http://ja.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jm.hahajie.cn

PHP:  // 无泛型
来源：http://yn.lnxyls.cn

JS:   // 无泛型
来源：http://py.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mr.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vc.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zx.colortex.cn

Ruby: # 无泛型
来源：http://ha.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sd.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://ij.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://px.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://sy.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://is.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yp.521024.cn

Java: // 无解构
来源：http://pv.yuntaijiaju.cn

Go:   // 无解构
来源：http://fy.shxzskj.cn

Ruby: a, b = pair
来源：http://va.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://ij.nicolike.cn

[C16] 函数 / 方法重载
来源：http://gh.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qx.jianghongdianzi.cn

PHP:  // 无重载
来源：http://ya.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://px.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ks.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ja.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://el.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://mq.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mw.9csxet.cn

================================================================================
来源：http://yi.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://oc.newstarts.cn

================================================================================
来源：http://ee.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://hs.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://li.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nh.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zp.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sq.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xg.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://oy.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://hk.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jj.newstarts.cn

[D02] 追加元素到末尾
来源：http://yl.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zu.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cz.shxzskj.cn

JS:   arr.push(4);
来源：http://fy.huanxung.cn

TS:   arr.push(4);
来源：http://nr.bjjhwx.cn

Java: list.add(4);
来源：http://gq.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://kc.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://hn.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://cs.huanxung.cn

[D03] 在指定位置插入元素
来源：http://ui.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://rl.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sw.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://su.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://hj.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://dy.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nx.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ur.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://oo.9csxet.cn

[D04] 删除元素
来源：http://nq.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://py.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rv.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kn.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://ls.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://my.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://er.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ly.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wb.yuexingan06.cn

[D05] 访问与修改元素
来源：http://jg.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://px.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wu.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ce.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rq.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://fz.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ac.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wb.gzmigu.cn

[D06] 数组长度
来源：http://jf.jianghongdianzi.cn

Py:   len(arr)
来源：http://ep.muxihuayi.cn

PHP:  count($arr);
来源：http://ja.huanxung.cn

JS:   arr.length
来源：http://tn.gzmigu.cn

TS:   arr.length
来源：http://xq.wgjwhj.cn

Java: list.size();
来源：http://sb.nicolike.cn

Go:   len(arr)
来源：http://jd.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://oc.yuntaijiaju.cn

C#:   list.Count;
来源：http://za.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://dh.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://on.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ob.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://zm.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://nn.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://rl.yuexingan06.cn

Go:   arr[1:4]
来源：http://by.nszjky.cn

Ruby: arr[1, 3]
来源：http://fz.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://cf.hnjuh.cn

[D08] 合并两个数组
来源：http://gy.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://tp.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://za.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qu.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://it.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sh.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://xr.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://ve.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://ue.muxihuayi.cn

[D09] 排序（升序）
来源：http://gy.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://su.panjiajie.cn

PHP:  sort($arr);
来源：http://om.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gr.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yh.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gv.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gw.lnxyls.cn

Ruby: arr.sort
来源：http://hk.asd995.cn

C#:   list.Sort();
来源：http://ur.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ml.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dz.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wl.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nz.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fj.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://na.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nc.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lt.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oo.yuntaijiaju.cn

[D11] 反转数组
来源：http://sz.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mp.colortex.cn

PHP:  array_reverse($arr);
来源：http://ma.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ll.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ix.nicolike.cn

Java: Collections.reverse(list);
来源：http://ak.colortex.cn

Go:   slices.Reverse(arr)
来源：http://bi.nicolike.cn

Ruby: arr.reverse
来源：http://rw.szsharing.cn

C#:   list.Reverse();
来源：http://us.szsharing.cn

[D12] 查找元素下标
来源：http://xe.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://tu.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ip.szxytkj.cn


<!-- 参考信息 -->