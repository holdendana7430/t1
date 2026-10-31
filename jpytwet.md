代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://va.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kv.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vo.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dn.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ne.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://ou.asd995.cn

PHP:  is_numeric($x)
来源：http://lp.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cc.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ff.nszjky.cn

Java: x instanceof Number
来源：http://lk.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ke.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://hf.521024.cn

C#:   x is int or double or decimal
来源：http://pf.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ea.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sq.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hc.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://rn.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://kn.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vh.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lp.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uk.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pd.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://vj.jctech888.com.cn

Py:   a and b or not c
来源：http://jv.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://nm.szxytkj.cn

JS:   a && b || !c
来源：http://yh.chemitech.net.cn

TS:   a && b || !c
来源：http://zq.haigaiapp.cn

Java: a && b || !c
来源：http://oe.huixinmuqiang.cn

Go:   a && b || !c
来源：http://kn.lnxyls.cn

Ruby: a && b || !c
来源：http://ai.asd995.cn

C#:   a && b || !c
来源：http://nu.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uc.jctech888.com.cn

Py:   if not data: return
来源：http://iq.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://yb.hnjuh.cn

JS:   if (!data) return;
来源：http://xe.lnxyls.cn

TS:   if (!data) return;
来源：http://nw.bjjhwx.cn

Java: if (data == null) return;
来源：http://qi.hnjuh.cn

Go:   if data == nil { return }
来源：http://ld.huixiangedu.cn

Ruby: return if data.nil?
来源：http://hj.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://xi.haigaiapp.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

C. 函数与作用域
来源：http://vo.9csxet.cn

================================================================================
来源：http://gv.colortex.cn

[C01] 定义函数
来源：http://gc.asd995.cn

Py:   def add(a, b): return a + b
来源：http://za.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ry.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://tu.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ox.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tt.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dn.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://fb.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rw.yuntaijiaju.cn

[C02] 默认参数
来源：http://ax.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://tj.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iv.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://mt.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lw.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kb.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ro.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://cw.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gw.shxzukj.cn

[C03] 可变参数
来源：http://gt.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://og.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fl.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zm.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yu.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pb.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dk.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ik.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xa.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://le.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ab.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ch.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ts.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rd.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ec.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://jd.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://kn.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ye.yuexingan06.cn

[C05] 返回多个值
来源：http://ab.nszjky.cn

Py:   return a, b
来源：http://pd.szsharing.cn

PHP:  return [$a, $b];
来源：http://xy.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rr.gzmigu.cn

TS:   return { a, b };
来源：http://ob.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nd.muxihuayi.cn

Go:   return a, b
来源：http://bv.hnjuh.cn

Ruby: return a, b
来源：http://ai.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ap.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://gp.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://rh.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rl.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://cg.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://vb.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bd.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://we.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://in.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dc.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://wf.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dn.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://el.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qd.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://wh.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mv.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jo.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://se.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iz.colortex.cn

[C08] 闭包
来源：http://ce.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mn.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gm.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qw.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sg.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ji.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nw.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sc.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tc.521024.cn

[C09] 递归
来源：http://wk.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tw.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uo.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zr.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xp.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xu.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://go.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://or.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cf.shxzskj.cn

[C10] 变量作用域
来源：http://su.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sd.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hv.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ma.asd995.cn

TS:   同 JS
来源：http://ay.hahajie.cn

Java: 方法内为块级作用域
来源：http://hn.shxzskj.cn

Go:   花括号块级作用域
来源：http://at.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xw.nicolike.cn

C#:   块级作用域
来源：http://ro.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://be.huanxung.cn

Py:   from module import func
来源：http://nf.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yt.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bi.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vq.yuexingan06.cn

Java: import java.util.List;
来源：http://lp.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vl.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://fy.newstarts.cn

C#:   using System.Text;
来源：http://jj.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://ql.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ap.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://zg.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://no.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://di.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jx.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gb.521024.cn

Ruby: -> { puts "run" }.call
来源：http://aw.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://st.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://eo.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sa.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zu.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rw.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rb.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vk.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://uf.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ur.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lb.haigaiapp.cn

[C14] 泛型函数
来源：http://tf.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sc.panjiajie.cn

PHP:  // 无泛型
来源：http://cd.chemitech.net.cn

JS:   // 无泛型
来源：http://nl.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lu.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wn.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yp.bookmarksfly.cn

Ruby: # 无泛型
来源：http://oc.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://td.hahajie.cn

[C15] 解构 / 展开参数
来源：http://kh.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ol.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://qs.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tb.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fg.521024.cn

Java: // 无解构
来源：http://sq.jianghongdianzi.cn

Go:   // 无解构
来源：http://xr.shxzskj.cn

Ruby: a, b = pair
来源：http://pk.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://av.hahajie.cn

[C16] 函数 / 方法重载
来源：http://mq.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wu.gzmigu.cn

PHP:  // 无重载
来源：http://yu.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eb.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://iz.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lq.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://an.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://dc.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://va.huixiangedu.cn

================================================================================
来源：http://xl.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://hi.nicolike.cn

================================================================================
来源：http://ud.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://ai.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ct.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://di.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://py.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ri.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gx.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://cg.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://zu.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pr.szsharing.cn

[D02] 追加元素到末尾
来源：http://pv.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gc.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bk.chemitech.net.cn

JS:   arr.push(4);
来源：http://wt.bookmarksfly.cn

TS:   arr.push(4);
来源：http://sl.bookmarksfly.cn

Java: list.add(4);
来源：http://rk.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://cb.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ts.huixiangedu.cn

C#:   list.Add(4);
来源：http://xj.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://zl.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://vd.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lz.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zp.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://pp.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://uw.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vp.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://su.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://tf.asd995.cn

[D04] 删除元素
来源：http://nn.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qy.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://me.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://px.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://kd.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://op.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ei.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hq.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bb.lnxyls.cn

[D05] 访问与修改元素
来源：http://ed.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xp.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://an.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nf.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://za.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://gk.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://xz.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xf.hnjuh.cn

[D06] 数组长度
来源：http://xs.shtwfgs.cn

Py:   len(arr)
来源：http://wa.9csxet.cn

PHP:  count($arr);
来源：http://fm.newstarts.cn

JS:   arr.length
来源：http://xy.jianghongdianzi.cn

TS:   arr.length
来源：http://nz.yuexingan06.cn

Java: list.size();
来源：http://xd.wgjwhj.cn

Go:   len(arr)
来源：http://pk.asd995.cn

Ruby: arr.length; arr.size
来源：http://gl.9csxet.cn

C#:   list.Count;
来源：http://yk.hahajie.cn

[D07] 切片 / 取子数组
来源：http://rl.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bv.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ve.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://px.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://wh.panjiajie.cn

Java: list.subList(1, 4);
来源：http://gr.panjiajie.cn

Go:   arr[1:4]
来源：http://xm.nicolike.cn

Ruby: arr[1, 3]
来源：http://ca.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://mc.bjjhwx.cn

[D08] 合并两个数组
来源：http://gt.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://xx.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ll.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fy.yuexingan06.cn

TS:   [...a, ...b];
来源：http://yl.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zd.haigaiapp.cn

Go:   append(a, b...)
来源：http://oz.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://hv.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://ya.9csxet.cn

[D09] 排序（升序）
来源：http://ot.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://iw.jctech888.com.cn

PHP:  sort($arr);
来源：http://jv.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pt.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://io.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://re.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hg.shxzukj.cn

Ruby: arr.sort
来源：http://xp.nicolike.cn

C#:   list.Sort();
来源：http://xd.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ee.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ri.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ee.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pp.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ci.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uq.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eg.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cy.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xe.nicolike.cn

[D11] 反转数组
来源：http://yj.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://na.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://jf.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ld.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://xh.panjiajie.cn

Java: Collections.reverse(list);
来源：http://ii.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://hf.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://tq.bookmarksfly.cn

C#:   list.Reverse();
来源：http://gu.lnxyls.cn

[D12] 查找元素下标
来源：http://bt.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://bv.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ns.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vh.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ve.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oy.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://zr.asd995.cn

Ruby: arr.index(x)
来源：http://zs.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://oz.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://lb.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ad.lnxyls.cn


<!-- 参考信息 -->