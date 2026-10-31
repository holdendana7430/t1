代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://oc.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://va.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wn.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cy.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ef.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qx.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ik.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pe.chemitech.net.cn

[B13] 判断是否为数字
来源：http://dh.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://km.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://xv.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ff.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gd.shxzskj.cn

Java: x instanceof Number
来源：http://cw.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tl.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://qp.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ia.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://fg.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gc.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pd.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://jr.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://dt.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cu.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dp.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fn.gzmigu.cn

[B15] 布尔运算与取反
来源：http://it.chemitech.net.cn

Py:   a and b or not c
来源：http://yv.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://wo.yuntaijiaju.cn

JS:   a && b || !c
来源：http://jb.shtwfgs.cn

TS:   a && b || !c
来源：http://es.huixinmuqiang.cn

Java: a && b || !c
来源：http://px.hnjuh.cn

Go:   a && b || !c
来源：http://hd.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://rj.newstarts.cn

C#:   a && b || !c
来源：http://po.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ip.huixinmuqiang.cn

Py:   if not data: return
来源：http://zv.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://gu.nicolike.cn

JS:   if (!data) return;
来源：http://fc.haigaiapp.cn

TS:   if (!data) return;
来源：http://km.bookmarksfly.cn

Java: if (data == null) return;
来源：http://xh.jctech888.com.cn

Go:   if data == nil { return }
来源：http://rf.colortex.cn

Ruby: return if data.nil?
来源：http://ul.lnxyls.cn

C#:   if (data == null) return;
来源：http://ia.szxytkj.cn

================================================================================
来源：http://wu.yuntaijiaju.cn

C. 函数与作用域
来源：http://ww.bjjhwx.cn

================================================================================
来源：http://uv.shxzukj.cn

[C01] 定义函数
来源：http://dk.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://br.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://rm.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mc.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wu.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ch.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://hl.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bz.nszjky.cn

[C02] 默认参数
来源：http://yp.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://cd.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yb.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://gi.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ca.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://px.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gf.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://gh.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://cr.asd995.cn

[C03] 可变参数
来源：http://or.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ao.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sl.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uq.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pz.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ol.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xo.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ys.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qu.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://cq.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ks.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sp.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gu.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uc.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://fz.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://ny.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://pi.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://wl.szxytkj.cn

[C05] 返回多个值
来源：http://yu.szsharing.cn

Py:   return a, b
来源：http://kg.shxzukj.cn

PHP:  return [$a, $b];
来源：http://zq.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dn.shxzukj.cn

TS:   return { a, b };
来源：http://ih.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jz.nszjky.cn

Go:   return a, b
来源：http://of.newstarts.cn

Ruby: return a, b
来源：http://tc.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://fh.colortex.cn

[C06] 匿名函数 / lambda
来源：http://so.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://tn.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://um.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://cf.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://sx.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cw.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jt.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://zm.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xh.521024.cn

[C07] 把函数作为参数传入
来源：http://je.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hr.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://we.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rb.szxytkj.cn

TS:   arr.map(String)
来源：http://es.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zg.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://an.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://og.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qi.nicolike.cn

[C08] 闭包
来源：http://ek.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://le.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sg.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lp.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fc.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ds.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://km.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://px.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sg.szxytkj.cn

[C09] 递归
来源：http://rq.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mt.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kr.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fl.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kg.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xh.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ap.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://le.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vy.bookmarksfly.cn

[C10] 变量作用域
来源：http://ut.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ho.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jv.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jp.huixinmuqiang.cn

TS:   同 JS
来源：http://lu.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://ef.gzmigu.cn

Go:   花括号块级作用域
来源：http://xq.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pa.colortex.cn

C#:   块级作用域
来源：http://vk.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ji.bjjhwx.cn

Py:   from module import func
来源：http://et.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hi.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zt.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ir.lnxyls.cn

Java: import java.util.List;
来源：http://xd.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dy.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://be.jctech888.com.cn

C#:   using System.Text;
来源：http://ex.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://to.colortex.cn

Py:   (lambda: print("run"))()
来源：http://vb.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://pl.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://pe.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://jq.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bq.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yj.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://gk.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ho.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://rd.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bk.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qy.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yp.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fd.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vj.hahajie.cn

Go:   func add(a, b int) int
来源：http://zf.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gn.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mp.yuexingan06.cn

[C14] 泛型函数
来源：http://wt.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ne.yuexingan06.cn

PHP:  // 无泛型
来源：http://es.hnjuh.cn

JS:   // 无泛型
来源：http://xu.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vd.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dn.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hn.shxzukj.cn

Ruby: # 无泛型
来源：http://yo.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gt.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://jj.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nj.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://su.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nj.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fn.huixinmuqiang.cn

Java: // 无解构
来源：http://jl.lnxyls.cn

Go:   // 无解构
来源：http://ta.hahajie.cn

Ruby: a, b = pair
来源：http://rc.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://qr.nszjky.cn

[C16] 函数 / 方法重载
来源：http://ca.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jc.muxihuayi.cn

PHP:  // 无重载
来源：http://ab.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uq.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://gy.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ds.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ag.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ow.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fr.szsharing.cn

================================================================================
来源：http://co.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://ag.huixinmuqiang.cn

================================================================================
来源：http://dj.521024.cn

[D01] 创建数组 / 列表
来源：http://kc.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kv.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gi.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cg.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qg.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hl.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://gw.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://sq.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nv.nicolike.cn

[D02] 追加元素到末尾
来源：http://tr.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vw.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lk.hahajie.cn

JS:   arr.push(4);
来源：http://yl.asd995.cn

TS:   arr.push(4);
来源：http://yg.wgjwhj.cn

Java: list.add(4);
来源：http://wj.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://pg.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://op.haigaiapp.cn

C#:   list.Add(4);
来源：http://zz.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://yu.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://tq.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kb.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://or.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://xu.hnjuh.cn

Java: list.add(0, 0);
来源：http://tn.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://or.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yr.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://bl.huanxung.cn

[D04] 删除元素
来源：http://we.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ud.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fq.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lx.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://gl.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cn.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vh.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oq.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cw.lnxyls.cn

[D05] 访问与修改元素
来源：http://pd.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zf.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tx.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ay.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://qu.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://og.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://az.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cm.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gz.shtwfgs.cn

[D06] 数组长度
来源：http://gf.colortex.cn

Py:   len(arr)
来源：http://os.szxytkj.cn

PHP:  count($arr);
来源：http://le.nszjky.cn

JS:   arr.length
来源：http://ds.huixiangedu.cn

TS:   arr.length
来源：http://sy.huixinmuqiang.cn

Java: list.size();
来源：http://gy.9csxet.cn

Go:   len(arr)
来源：http://ht.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://yr.nicolike.cn

C#:   list.Count;
来源：http://uu.newstarts.cn

[D07] 切片 / 取子数组
来源：http://lu.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eh.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rp.asd995.cn

JS:   arr.slice(1, 4);
来源：http://pj.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://lo.nszjky.cn

Java: list.subList(1, 4);
来源：http://lb.szxytkj.cn

Go:   arr[1:4]
来源：http://xc.gzmigu.cn

Ruby: arr[1, 3]
来源：http://eo.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://fo.jctech888.com.cn

[D08] 合并两个数组
来源：http://we.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://lq.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://we.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ta.asd995.cn

TS:   [...a, ...b];
来源：http://un.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dh.shxzukj.cn

Go:   append(a, b...)
来源：http://pd.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://ha.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://hz.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://xx.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.hnjuh.cn

PHP:  sort($arr);
来源：http://zk.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ht.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qb.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hy.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fc.asd995.cn

Ruby: arr.sort
来源：http://em.colortex.cn

C#:   list.Sort();
来源：http://sy.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ue.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nr.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ts.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cd.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://on.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wy.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lt.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jp.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kv.huanxung.cn

[D11] 反转数组
来源：http://lp.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ck.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://fn.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zo.hnjuh.cn

TS:   [...arr].reverse();
来源：http://aq.nszjky.cn

Java: Collections.reverse(list);
来源：http://pe.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://yo.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://xm.chemitech.net.cn

C#:   list.Reverse();
来源：http://ak.muxihuayi.cn

[D12] 查找元素下标
来源：http://ou.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://me.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ij.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mb.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ui.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qe.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://pc.yuntaijiaju.cn


<!-- 参考信息 -->