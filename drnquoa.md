代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zm.521024.cn

Java: x instanceof Number
来源：http://bt.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ir.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://aw.nszjky.cn

C#:   x is int or double or decimal
来源：http://nz.newstarts.cn

[B14] 判断值是否在集合内
来源：http://xj.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uk.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wr.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://oi.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ym.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ty.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hg.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://od.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rj.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ih.haigaiapp.cn

Py:   a and b or not c
来源：http://yc.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://sg.hnjuh.cn

JS:   a && b || !c
来源：http://oo.jctech888.com.cn

TS:   a && b || !c
来源：http://bp.wgjwhj.cn

Java: a && b || !c
来源：http://nr.521024.cn

Go:   a && b || !c
来源：http://rg.huanxung.cn

Ruby: a && b || !c
来源：http://yc.muxihuayi.cn

C#:   a && b || !c
来源：http://hv.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vs.asd995.cn

Py:   if not data: return
来源：http://aw.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://vf.asd995.cn

JS:   if (!data) return;
来源：http://bg.wgjwhj.cn

TS:   if (!data) return;
来源：http://sz.9csxet.cn

Java: if (data == null) return;
来源：http://vy.521024.cn

Go:   if data == nil { return }
来源：http://tp.haigaiapp.cn

Ruby: return if data.nil?
来源：http://bp.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://jc.wgjwhj.cn

================================================================================
来源：http://ml.nicolike.cn

C. 函数与作用域
来源：http://jk.yuexingan06.cn

================================================================================
来源：http://vz.huanxung.cn

[C01] 定义函数
来源：http://fq.asd995.cn

Py:   def add(a, b): return a + b
来源：http://qa.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://mo.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rk.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ge.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rk.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://lt.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yg.gzmigu.cn

[C02] 默认参数
来源：http://qv.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://yt.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ce.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://wy.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wt.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ew.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gh.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://ex.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://tn.hahajie.cn

[C03] 可变参数
来源：http://qa.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://qv.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yi.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tu.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ng.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pb.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ce.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pe.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pl.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://ou.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nz.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pq.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kk.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dp.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://fi.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://vx.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ob.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://ap.hahajie.cn

[C05] 返回多个值
来源：http://ra.521024.cn

Py:   return a, b
来源：http://up.newstarts.cn

PHP:  return [$a, $b];
来源：http://tx.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://km.huanxung.cn

TS:   return { a, b };
来源：http://kn.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bm.newstarts.cn

Go:   return a, b
来源：http://fw.hnjuh.cn

Ruby: return a, b
来源：http://bk.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://pc.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ru.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://gj.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ci.shxzskj.cn

JS:   const square = x => x * x;
来源：http://ul.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://mn.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://py.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://db.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://zm.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ze.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://cu.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://az.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nt.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dm.hahajie.cn

TS:   arr.map(String)
来源：http://ho.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cs.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://kj.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eb.521024.cn

[C08] 闭包
来源：http://ar.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zl.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gk.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tt.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ja.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fm.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://so.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yn.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qi.nszjky.cn

[C09] 递归
来源：http://gp.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://af.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yj.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zi.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gv.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oj.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://li.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://df.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fi.szxytkj.cn

[C10] 变量作用域
来源：http://pe.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vq.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pe.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gg.hahajie.cn

TS:   同 JS
来源：http://lp.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ib.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://yz.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qb.bjjhwx.cn

C#:   块级作用域
来源：http://qw.huanxung.cn

[C11] 模块导入与导出
来源：http://zu.szxytkj.cn

Py:   from module import func
来源：http://zj.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ng.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mb.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vs.jctech888.com.cn

Java: import java.util.List;
来源：http://ug.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vg.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://rf.jianghongdianzi.cn

C#:   using System.Text;
来源：http://eu.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://zk.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://mw.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://ui.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://wr.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://fa.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ma.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://vg.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://gb.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bt.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ua.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://si.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fx.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qc.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mm.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://pk.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fz.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bv.521024.cn

[C14] 泛型函数
来源：http://nx.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://et.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://ai.9csxet.cn

JS:   // 无泛型
来源：http://fa.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mr.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qo.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fa.bookmarksfly.cn

Ruby: # 无泛型
来源：http://cb.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eh.szsharing.cn

[C15] 解构 / 展开参数
来源：http://cl.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yl.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://mg.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uh.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gt.nicolike.cn

Java: // 无解构
来源：http://yg.shxzskj.cn

Go:   // 无解构
来源：http://va.521024.cn

Ruby: a, b = pair
来源：http://yu.521024.cn

C#:   var (a, b) = pair;
来源：http://kq.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://xn.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gr.jctech888.com.cn

PHP:  // 无重载
来源：http://zo.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ct.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://pe.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yp.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://fu.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://on.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fd.gzmigu.cn

================================================================================
来源：http://me.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://ul.shxzukj.cn

================================================================================
来源：http://fc.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://do.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qc.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://in.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ly.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fm.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fm.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://jc.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://rc.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zg.szsharing.cn

[D02] 追加元素到末尾
来源：http://wr.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cw.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jk.shxzskj.cn

JS:   arr.push(4);
来源：http://rf.szxytkj.cn

TS:   arr.push(4);
来源：http://xp.9csxet.cn

Java: list.add(4);
来源：http://hm.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://nl.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://kp.nicolike.cn

C#:   list.Add(4);
来源：http://ex.asd995.cn

[D03] 在指定位置插入元素
来源：http://zq.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://dk.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zu.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yo.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://sa.szxytkj.cn

Java: list.add(0, 0);
来源：http://hc.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bp.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jn.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://ep.szsharing.cn

[D04] 删除元素
来源：http://ab.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jm.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ka.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rm.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://ac.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nr.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ci.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nx.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ug.jctech888.com.cn

[D05] 访问与修改元素
来源：http://eo.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ei.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gu.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ce.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://rf.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://hf.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://mh.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://en.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://du.shtwfgs.cn

[D06] 数组长度
来源：http://sp.nicolike.cn

Py:   len(arr)
来源：http://hz.huixinmuqiang.cn

PHP:  count($arr);
来源：http://wb.521024.cn

JS:   arr.length
来源：http://gk.haigaiapp.cn

TS:   arr.length
来源：http://ol.asd995.cn

Java: list.size();
来源：http://fn.huanxung.cn

Go:   len(arr)
来源：http://zd.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://io.wgjwhj.cn

C#:   list.Count;
来源：http://bs.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://mh.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vk.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vp.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://in.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ed.colortex.cn

Java: list.subList(1, 4);
来源：http://yr.jctech888.com.cn

Go:   arr[1:4]
来源：http://ec.huanxung.cn

Ruby: arr[1, 3]
来源：http://qr.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://ua.muxihuayi.cn

[D08] 合并两个数组
来源：http://pi.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://pe.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://wr.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nb.shtwfgs.cn

TS:   [...a, ...b];
来源：http://dq.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://et.521024.cn

Go:   append(a, b...)
来源：http://kc.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://wk.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://zq.muxihuayi.cn

[D09] 排序（升序）
来源：http://or.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://lo.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qq.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qn.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tr.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://po.panjiajie.cn

Ruby: arr.sort
来源：http://zd.hnjuh.cn

C#:   list.Sort();
来源：http://of.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zh.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xt.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yt.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mw.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lu.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eo.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fe.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fl.huixinmuqiang.cn

[D11] 反转数组
来源：http://wt.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://an.newstarts.cn

PHP:  array_reverse($arr);
来源：http://qc.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jq.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://tt.521024.cn

Java: Collections.reverse(list);
来源：http://yg.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://qp.szxytkj.cn

Ruby: arr.reverse
来源：http://bm.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://qw.yuexingan06.cn

[D12] 查找元素下标
来源：http://tx.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://td.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mx.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kd.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wp.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://et.huixiangedu.cn

Ruby: arr.index(x)
来源：http://to.521024.cn

C#:   list.IndexOf(x);
来源：http://qn.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://kb.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pk.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fx.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://vo.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://jf.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ig.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qq.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ob.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oi.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://tl.yuexingan06.cn


<!-- 参考信息 -->