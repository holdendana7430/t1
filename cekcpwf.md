代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yn.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bf.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ou.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hj.9csxet.cn

[B13] 判断是否为数字
来源：http://am.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ex.lnxyls.cn

PHP:  is_numeric($x)
来源：http://xk.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tb.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eg.lnxyls.cn

Java: x instanceof Number
来源：http://qw.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lu.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://kq.szsharing.cn

C#:   x is int or double or decimal
来源：http://yf.asd995.cn

[B14] 判断值是否在集合内
来源：http://gz.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://am.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://or.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://cu.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ew.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nt.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zv.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jq.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qr.szsharing.cn

[B15] 布尔运算与取反
来源：http://ue.9csxet.cn

Py:   a and b or not c
来源：http://bq.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://dw.521024.cn

JS:   a && b || !c
来源：http://ct.nicolike.cn

TS:   a && b || !c
来源：http://ph.panjiajie.cn

Java: a && b || !c
来源：http://lf.gzmigu.cn

Go:   a && b || !c
来源：http://ml.yuexingan06.cn

Ruby: a && b || !c
来源：http://ng.huanxung.cn

C#:   a && b || !c
来源：http://fp.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ul.nszjky.cn

Py:   if not data: return
来源：http://ma.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://yl.shtwfgs.cn

JS:   if (!data) return;
来源：http://zo.newstarts.cn

TS:   if (!data) return;
来源：http://nz.muxihuayi.cn

Java: if (data == null) return;
来源：http://gj.huixiangedu.cn

Go:   if data == nil { return }
来源：http://wh.shxzukj.cn

Ruby: return if data.nil?
来源：http://kq.521024.cn

C#:   if (data == null) return;
来源：http://gh.panjiajie.cn

================================================================================
来源：http://vi.hahajie.cn

C. 函数与作用域
来源：http://tg.wgjwhj.cn

================================================================================
来源：http://qg.yuexingan06.cn

[C01] 定义函数
来源：http://gm.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ay.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bs.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://nk.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mq.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ih.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sa.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://xh.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bd.nszjky.cn

[C02] 默认参数
来源：http://pk.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://nq.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://es.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://mn.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iu.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fs.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bq.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://vl.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://lk.yuexingan06.cn

[C03] 可变参数
来源：http://fb.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://hs.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qn.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ze.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sj.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qp.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uv.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rq.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zw.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://iq.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ne.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pk.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://do.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vj.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.521024.cn

Go:   // 无：用配置结构体参数
来源：http://uk.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://he.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ut.yuexingan06.cn

[C05] 返回多个值
来源：http://du.nicolike.cn

Py:   return a, b
来源：http://vw.huanxung.cn

PHP:  return [$a, $b];
来源：http://ol.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xj.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ac.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sc.521024.cn

Go:   return a, b
来源：http://ao.9csxet.cn

Ruby: return a, b
来源：http://mo.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://jd.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://kk.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://wf.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://su.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://my.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://yz.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uh.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://do.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://mz.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eg.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://qn.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yg.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gz.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qh.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://hc.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uz.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gy.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://jk.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ik.nicolike.cn

[C08] 闭包
来源：http://um.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fe.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uf.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ne.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ek.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iq.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ez.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rf.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yk.panjiajie.cn

[C09] 递归
来源：http://tq.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yc.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pt.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kf.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ne.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://po.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ki.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ku.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://na.haigaiapp.cn

[C10] 变量作用域
来源：http://tj.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wt.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gt.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eh.nicolike.cn

TS:   同 JS
来源：http://nz.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://qt.newstarts.cn

Go:   花括号块级作用域
来源：http://pb.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hb.bookmarksfly.cn

C#:   块级作用域
来源：http://rp.hnjuh.cn

[C11] 模块导入与导出
来源：http://ap.huixinmuqiang.cn

Py:   from module import func
来源：http://ug.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dl.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pn.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qx.shxzskj.cn

Java: import java.util.List;
来源：http://jc.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oz.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://dv.shxzukj.cn

C#:   using System.Text;
来源：http://tn.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://mi.asd995.cn

Py:   (lambda: print("run"))()
来源：http://hy.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://sg.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://vl.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://hb.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zo.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://wi.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://aw.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zh.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://hw.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aq.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://om.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://op.nszjky.cn

Go:   func add(a, b int) int
来源：http://mf.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hw.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xx.jianghongdianzi.cn

[C14] 泛型函数
来源：http://bt.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nr.colortex.cn

PHP:  // 无泛型
来源：http://ff.nszjky.cn

JS:   // 无泛型
来源：http://os.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jn.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dp.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wh.asd995.cn

Ruby: # 无泛型
来源：http://he.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vs.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://cq.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bc.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://qk.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nh.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wj.asd995.cn

Java: // 无解构
来源：http://if.colortex.cn

Go:   // 无解构
来源：http://nt.nicolike.cn

Ruby: a, b = pair
来源：http://qj.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://zd.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://pt.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mu.shxzskj.cn

PHP:  // 无重载
来源：http://om.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zq.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://wb.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tp.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ia.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://jg.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sq.hnjuh.cn

================================================================================
来源：http://cg.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://pr.bjjhwx.cn

================================================================================
来源：http://la.nicolike.cn

[D01] 创建数组 / 列表
来源：http://oa.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ig.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ec.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pz.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hq.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ou.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://tz.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://mx.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nu.9csxet.cn

[D02] 追加元素到末尾
来源：http://nb.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mh.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://st.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://nc.hnjuh.cn

TS:   arr.push(4);
来源：http://os.521024.cn

Java: list.add(4);
来源：http://xh.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ax.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://my.muxihuayi.cn

C#:   list.Add(4);
来源：http://dh.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://jg.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://kx.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mm.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fx.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://pq.bjjhwx.cn

Java: list.add(0, 0);
来源：http://bl.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yk.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uz.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://nu.jctech888.com.cn

[D04] 删除元素
来源：http://la.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hu.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://th.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nf.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ei.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gu.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zs.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iw.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ag.huixiangedu.cn

[D05] 访问与修改元素
来源：http://kt.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://of.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ny.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qc.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ze.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://lt.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://xb.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bz.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gd.panjiajie.cn

[D06] 数组长度
来源：http://df.gzmigu.cn

Py:   len(arr)
来源：http://ap.lnxyls.cn

PHP:  count($arr);
来源：http://kt.hahajie.cn

JS:   arr.length
来源：http://wd.hahajie.cn

TS:   arr.length
来源：http://nx.gzmigu.cn

Java: list.size();
来源：http://up.szxytkj.cn

Go:   len(arr)
来源：http://rb.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ft.jctech888.com.cn

C#:   list.Count;
来源：http://dd.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://hd.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://js.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ua.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://cu.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ih.nicolike.cn

Java: list.subList(1, 4);
来源：http://ql.jctech888.com.cn

Go:   arr[1:4]
来源：http://ys.nszjky.cn

Ruby: arr[1, 3]
来源：http://hn.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://es.jctech888.com.cn

[D08] 合并两个数组
来源：http://qm.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://hq.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://fb.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tp.nszjky.cn

TS:   [...a, ...b];
来源：http://tm.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jf.9csxet.cn

Go:   append(a, b...)
来源：http://gu.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://ea.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://pe.hahajie.cn

[D09] 排序（升序）
来源：http://ud.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://fc.newstarts.cn

PHP:  sort($arr);
来源：http://ru.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xh.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ux.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bn.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ea.bjjhwx.cn

Ruby: arr.sort
来源：http://qj.yuntaijiaju.cn

C#:   list.Sort();
来源：http://wb.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://or.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yx.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://da.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jp.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qq.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yo.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ym.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tk.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sm.huixinmuqiang.cn

[D11] 反转数组
来源：http://vd.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ia.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://xg.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dh.asd995.cn

TS:   [...arr].reverse();
来源：http://uq.colortex.cn

Java: Collections.reverse(list);
来源：http://wm.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://nm.shxzskj.cn

Ruby: arr.reverse
来源：http://cr.hnjuh.cn

C#:   list.Reverse();
来源：http://hx.szxytkj.cn

[D12] 查找元素下标
来源：http://uf.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://vg.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ye.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://na.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lr.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://gs.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://ih.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://at.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://mr.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://la.newstarts.cn


<!-- 参考信息 -->