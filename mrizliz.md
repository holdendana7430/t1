代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kh.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ws.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lh.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tb.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pw.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://my.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://bh.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ps.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://aq.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sp.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ld.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cz.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zj.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://ix.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pp.yuexingan06.cn

[B12] 跳出多层循环
来源：http://rm.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xy.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cy.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nl.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ka.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yk.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uk.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rg.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jv.hnjuh.cn

[B13] 判断是否为数字
来源：http://vv.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://nn.gzmigu.cn

PHP:  is_numeric($x)
来源：http://pt.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hf.jctech888.com.cn

Java: x instanceof Number
来源：http://pr.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sz.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://cj.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://qe.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://gx.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qz.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yw.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://ds.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://zd.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ai.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tl.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ev.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ap.9csxet.cn

[B15] 布尔运算与取反
来源：http://ww.colortex.cn

Py:   a and b or not c
来源：http://yx.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ek.huixiangedu.cn

JS:   a && b || !c
来源：http://kn.lnxyls.cn

TS:   a && b || !c
来源：http://ry.panjiajie.cn

Java: a && b || !c
来源：http://jb.lnxyls.cn

Go:   a && b || !c
来源：http://dq.bookmarksfly.cn

Ruby: a && b || !c
来源：http://br.gzmigu.cn

C#:   a && b || !c
来源：http://zs.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tu.hahajie.cn

Py:   if not data: return
来源：http://pg.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://fe.huixiangedu.cn

JS:   if (!data) return;
来源：http://yf.haigaiapp.cn

TS:   if (!data) return;
来源：http://wq.asd995.cn

Java: if (data == null) return;
来源：http://eu.shtwfgs.cn

Go:   if data == nil { return }
来源：http://ar.huanxung.cn

Ruby: return if data.nil?
来源：http://eo.haigaiapp.cn

C#:   if (data == null) return;
来源：http://bh.jianghongdianzi.cn

================================================================================
来源：http://jb.shtwfgs.cn

C. 函数与作用域
来源：http://ez.hnjuh.cn

================================================================================
来源：http://do.newstarts.cn

[C01] 定义函数
来源：http://tb.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://dt.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jg.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://jr.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ic.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fa.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cp.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://qh.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vw.wgjwhj.cn

[C02] 默认参数
来源：http://fe.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://qh.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sv.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://xh.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pf.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cc.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xv.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://fe.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://se.szxytkj.cn

[C03] 可变参数
来源：http://yk.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://by.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hf.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wh.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oj.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eo.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nt.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://et.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://co.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://gf.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rj.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qq.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://we.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pq.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://vo.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://kc.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://sy.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://zj.huixiangedu.cn

[C05] 返回多个值
来源：http://iv.szxytkj.cn

Py:   return a, b
来源：http://hq.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://qd.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kz.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ms.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qa.nicolike.cn

Go:   return a, b
来源：http://fe.jctech888.com.cn

Ruby: return a, b
来源：http://ah.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://ui.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://eb.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://uo.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iz.hahajie.cn

JS:   const square = x => x * x;
来源：http://mn.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://gq.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ek.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eh.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://nl.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tq.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jf.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pj.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jw.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hm.bjjhwx.cn

TS:   arr.map(String)
来源：http://yi.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ag.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://de.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://un.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fx.shtwfgs.cn

[C08] 闭包
来源：http://nh.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kr.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kz.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nr.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dq.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hf.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zp.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://so.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ea.wgjwhj.cn

[C09] 递归
来源：http://kv.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vb.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mc.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sx.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ws.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sm.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://da.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hl.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ek.shxzskj.cn

[C10] 变量作用域
来源：http://jb.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mh.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://av.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tv.shtwfgs.cn

TS:   同 JS
来源：http://bf.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ap.haigaiapp.cn

Go:   花括号块级作用域
来源：http://tv.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jq.hahajie.cn

C#:   块级作用域
来源：http://by.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://cl.colortex.cn

Py:   from module import func
来源：http://nq.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ru.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sw.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zo.yuntaijiaju.cn

Java: import java.util.List;
来源：http://ne.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mj.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://np.newstarts.cn

C#:   using System.Text;
来源：http://hx.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ny.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://zb.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://bo.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://vq.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://ub.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://nv.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://pl.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mw.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://uy.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xb.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wi.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sr.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jl.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://in.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://av.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wu.haigaiapp.cn

[C14] 泛型函数
来源：http://ar.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ol.shxzskj.cn

PHP:  // 无泛型
来源：http://jt.wgjwhj.cn

JS:   // 无泛型
来源：http://ql.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://et.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ck.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.shxzskj.cn

Ruby: # 无泛型
来源：http://bc.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mw.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://si.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hm.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ms.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ib.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://av.haigaiapp.cn

Java: // 无解构
来源：http://rd.yuexingan06.cn

Go:   // 无解构
来源：http://ns.panjiajie.cn

Ruby: a, b = pair
来源：http://is.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://zu.nicolike.cn

[C16] 函数 / 方法重载
来源：http://wl.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bq.hnjuh.cn

PHP:  // 无重载
来源：http://ax.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sj.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://gr.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jj.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ak.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://dn.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ik.yuexingan06.cn

================================================================================
来源：http://rg.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ef.yuexingan06.cn

================================================================================
来源：http://yx.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://sh.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oo.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ws.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lh.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cd.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ba.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://on.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://go.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pj.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://fb.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ys.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://px.gzmigu.cn

JS:   arr.push(4);
来源：http://pd.colortex.cn

TS:   arr.push(4);
来源：http://ky.jctech888.com.cn

Java: list.add(4);
来源：http://dg.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://hk.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://pc.gzmigu.cn

C#:   list.Add(4);
来源：http://pb.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://gz.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://cx.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://og.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fy.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://er.szxytkj.cn

Java: list.add(0, 0);
来源：http://hx.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gl.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wo.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://nc.shxzskj.cn

[D04] 删除元素
来源：http://us.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rp.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tm.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://hp.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://am.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nr.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ch.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ub.9csxet.cn

[D05] 访问与修改元素
来源：http://ch.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vf.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pq.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fw.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://zv.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://um.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://wv.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xk.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ec.nicolike.cn

[D06] 数组长度
来源：http://fs.wgjwhj.cn

Py:   len(arr)
来源：http://pc.panjiajie.cn

PHP:  count($arr);
来源：http://wl.521024.cn

JS:   arr.length
来源：http://mu.521024.cn

TS:   arr.length
来源：http://pz.yuexingan06.cn

Java: list.size();
来源：http://rc.newstarts.cn

Go:   len(arr)
来源：http://fk.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://zn.huixinmuqiang.cn

C#:   list.Count;
来源：http://pv.nszjky.cn

[D07] 切片 / 取子数组
来源：http://op.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eq.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mz.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://mq.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://oj.szxytkj.cn

Java: list.subList(1, 4);
来源：http://dj.jctech888.com.cn

Go:   arr[1:4]
来源：http://ys.9csxet.cn

Ruby: arr[1, 3]
来源：http://vv.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://cf.bjjhwx.cn

[D08] 合并两个数组
来源：http://ed.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://oi.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://sw.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://li.colortex.cn

TS:   [...a, ...b];
来源：http://zm.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rm.9csxet.cn

Go:   append(a, b...)
来源：http://aj.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://qd.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://mh.bookmarksfly.cn

[D09] 排序（升序）
来源：http://dk.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.shxzskj.cn

PHP:  sort($arr);
来源：http://zx.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lg.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cu.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gk.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dw.asd995.cn

Ruby: arr.sort
来源：http://kg.lnxyls.cn

C#:   list.Sort();
来源：http://aq.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fx.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iz.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bn.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cc.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vv.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://di.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iu.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eo.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fh.huixinmuqiang.cn


<!-- 参考信息 -->