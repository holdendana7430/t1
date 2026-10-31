代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://cj.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ki.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pq.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vr.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cx.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eo.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qg.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hf.nicolike.cn

[B13] 判断是否为数字
来源：http://kw.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://pr.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://hk.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sv.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uc.521024.cn

Java: x instanceof Number
来源：http://ip.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uh.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://oa.szxytkj.cn

C#:   x is int or double or decimal
来源：http://nt.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://ho.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sx.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bl.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://nm.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://dv.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nx.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://og.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oz.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cy.newstarts.cn

[B15] 布尔运算与取反
来源：http://vv.shxzskj.cn

Py:   a and b or not c
来源：http://nd.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://pj.nszjky.cn

JS:   a && b || !c
来源：http://tt.panjiajie.cn

TS:   a && b || !c
来源：http://lf.haigaiapp.cn

Java: a && b || !c
来源：http://it.jianghongdianzi.cn

Go:   a && b || !c
来源：http://qm.huanxung.cn

Ruby: a && b || !c
来源：http://xp.hahajie.cn

C#:   a && b || !c
来源：http://wr.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://el.chemitech.net.cn

Py:   if not data: return
来源：http://eq.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://rx.gzmigu.cn

JS:   if (!data) return;
来源：http://bh.huixiangedu.cn

TS:   if (!data) return;
来源：http://ac.shxzskj.cn

Java: if (data == null) return;
来源：http://wu.haigaiapp.cn

Go:   if data == nil { return }
来源：http://jp.hnjuh.cn

Ruby: return if data.nil?
来源：http://ti.szxytkj.cn

C#:   if (data == null) return;
来源：http://iu.huixiangedu.cn

================================================================================
来源：http://ws.jctech888.com.cn

C. 函数与作用域
来源：http://uv.chemitech.net.cn

================================================================================
来源：http://vk.hahajie.cn

[C01] 定义函数
来源：http://pj.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://fl.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://or.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://lp.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://my.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ze.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://le.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://ph.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nx.panjiajie.cn

[C02] 默认参数
来源：http://we.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://ei.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pa.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://dh.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gm.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sq.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ua.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://cs.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://yz.nszjky.cn

[C03] 可变参数
来源：http://qv.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ll.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://se.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://em.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://da.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wi.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ck.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://el.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lm.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://wt.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://re.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rk.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fj.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wm.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ko.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://xs.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://ol.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://yc.szsharing.cn

[C05] 返回多个值
来源：http://oh.shxzukj.cn

Py:   return a, b
来源：http://fq.szsharing.cn

PHP:  return [$a, $b];
来源：http://re.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lz.shtwfgs.cn

TS:   return { a, b };
来源：http://lw.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cy.9csxet.cn

Go:   return a, b
来源：http://kb.huanxung.cn

Ruby: return a, b
来源：http://tt.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://tb.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://mj.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://rm.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ld.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://hm.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://zt.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pr.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xe.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://lc.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fp.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://bi.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rs.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ay.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ac.colortex.cn

TS:   arr.map(String)
来源：http://nw.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hn.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kc.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://oe.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ox.bjjhwx.cn

[C08] 闭包
来源：http://zl.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gr.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ph.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lq.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hg.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xx.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mu.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://en.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ab.yuntaijiaju.cn

[C09] 递归
来源：http://qc.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fo.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bz.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wf.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tx.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tj.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ze.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yw.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jo.asd995.cn

[C10] 变量作用域
来源：http://nj.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://of.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ej.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pa.newstarts.cn

TS:   同 JS
来源：http://hn.nszjky.cn

Java: 方法内为块级作用域
来源：http://wu.nszjky.cn

Go:   花括号块级作用域
来源：http://vh.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hc.muxihuayi.cn

C#:   块级作用域
来源：http://oo.muxihuayi.cn

[C11] 模块导入与导出
来源：http://kd.521024.cn

Py:   from module import func
来源：http://yo.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nf.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qq.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://he.hnjuh.cn

Java: import java.util.List;
来源：http://te.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fg.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://nr.wgjwhj.cn

C#:   using System.Text;
来源：http://ip.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://mh.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://ox.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://av.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://tb.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://bt.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ue.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ba.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://vw.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ig.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://ct.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fj.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yv.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qs.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bc.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://zv.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iq.bookmarksfly.cn

[C14] 泛型函数
来源：http://uh.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rt.nszjky.cn

PHP:  // 无泛型
来源：http://dh.shtwfgs.cn

JS:   // 无泛型
来源：http://xi.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ga.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://um.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://py.haigaiapp.cn

Ruby: # 无泛型
来源：http://xp.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ce.521024.cn

[C15] 解构 / 展开参数
来源：http://ul.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bu.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://mp.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ad.colortex.cn

Java: // 无解构
来源：http://tp.huixinmuqiang.cn

Go:   // 无解构
来源：http://jg.chemitech.net.cn

Ruby: a, b = pair
来源：http://dz.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://fm.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://fh.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qo.newstarts.cn

PHP:  // 无重载
来源：http://ai.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uo.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ck.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sa.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://rd.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://hw.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xl.bjjhwx.cn

================================================================================
来源：http://yc.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://fb.bjjhwx.cn

================================================================================
来源：http://gz.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ng.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ie.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dr.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kz.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ks.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nn.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://ei.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://xg.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ux.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://lk.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kd.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lu.haigaiapp.cn

JS:   arr.push(4);
来源：http://tu.panjiajie.cn

TS:   arr.push(4);
来源：http://lr.huanxung.cn

Java: list.add(4);
来源：http://hz.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://bk.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://wz.hahajie.cn

C#:   list.Add(4);
来源：http://th.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://gw.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://mr.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bo.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jm.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://jy.huixiangedu.cn

Java: list.add(0, 0);
来源：http://kp.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://io.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oj.colortex.cn

C#:   list.Insert(0, 0);
来源：http://lk.panjiajie.cn

[D04] 删除元素
来源：http://wc.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uy.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rv.huixinmuqiang.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bj.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://rm.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aq.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rv.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sq.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ux.wgjwhj.cn

[D05] 访问与修改元素
来源：http://ps.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://os.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kq.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fk.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://lo.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://mt.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://yo.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rn.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lr.haigaiapp.cn

[D06] 数组长度
来源：http://wu.jctech888.com.cn

Py:   len(arr)
来源：http://pi.shtwfgs.cn

PHP:  count($arr);
来源：http://ck.huixinmuqiang.cn

JS:   arr.length
来源：http://on.muxihuayi.cn

TS:   arr.length
来源：http://as.haigaiapp.cn

Java: list.size();
来源：http://sg.bookmarksfly.cn

Go:   len(arr)
来源：http://zv.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://es.huixiangedu.cn

C#:   list.Count;
来源：http://at.521024.cn

[D07] 切片 / 取子数组
来源：http://tu.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qf.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cq.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://hh.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://dd.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ci.chemitech.net.cn

Go:   arr[1:4]
来源：http://cj.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://vv.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://gj.colortex.cn

[D08] 合并两个数组
来源：http://gb.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://se.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://ok.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wc.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://gv.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cv.lnxyls.cn

Go:   append(a, b...)
来源：http://br.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://vc.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://cx.nszjky.cn

[D09] 排序（升序）
来源：http://zx.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://mz.wgjwhj.cn

PHP:  sort($arr);
来源：http://ly.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qz.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ka.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wb.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nz.newstarts.cn

Ruby: arr.sort
来源：http://hi.bjjhwx.cn

C#:   list.Sort();
来源：http://oy.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mz.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cb.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mg.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ea.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xw.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://im.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hd.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://js.asd995.cn

[D11] 反转数组
来源：http://yf.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://de.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://nb.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pk.asd995.cn

TS:   [...arr].reverse();
来源：http://yb.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://sp.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://zi.jctech888.com.cn

Ruby: arr.reverse
来源：http://sd.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://ny.asd995.cn

[D12] 查找元素下标
来源：http://ub.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://bh.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hb.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://la.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lu.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yp.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://lz.wgjwhj.cn


<!-- 参考信息 -->