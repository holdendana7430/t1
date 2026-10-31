代发 wailian999

PHP:  range(0, 10, 2);
来源：http://yf.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bw.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://na.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qi.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nx.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://qu.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xv.muxihuayi.cn

[B12] 跳出多层循环
来源：http://qo.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cm.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wc.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ry.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sf.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://za.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nc.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bt.szsharing.cn

[B13] 判断是否为数字
来源：http://ma.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://dd.asd995.cn

PHP:  is_numeric($x)
来源：http://po.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ms.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zn.hahajie.cn

Java: x instanceof Number
来源：http://cg.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ny.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ct.panjiajie.cn

C#:   x is int or double or decimal
来源：http://fd.hahajie.cn

[B14] 判断值是否在集合内
来源：http://lr.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://er.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ds.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://kf.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://dt.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://au.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kr.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bg.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fn.nicolike.cn

[B15] 布尔运算与取反
来源：http://jk.huixinmuqiang.cn

Py:   a and b or not c
来源：http://bi.colortex.cn

PHP:  $a && $b || !$c
来源：http://lm.gzmigu.cn

JS:   a && b || !c
来源：http://tj.szsharing.cn

TS:   a && b || !c
来源：http://lz.newstarts.cn

Java: a && b || !c
来源：http://tb.szsharing.cn

Go:   a && b || !c
来源：http://lr.nszjky.cn

Ruby: a && b || !c
来源：http://eg.yuntaijiaju.cn

C#:   a && b || !c
来源：http://nb.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://if.bjjhwx.cn

Py:   if not data: return
来源：http://jy.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://hp.yuexingan06.cn

JS:   if (!data) return;
来源：http://nl.chemitech.net.cn

TS:   if (!data) return;
来源：http://zo.muxihuayi.cn

Java: if (data == null) return;
来源：http://di.panjiajie.cn

Go:   if data == nil { return }
来源：http://uk.huanxung.cn

Ruby: return if data.nil?
来源：http://ca.colortex.cn

C#:   if (data == null) return;
来源：http://kf.hnjuh.cn

================================================================================
来源：http://dk.shxzskj.cn

C. 函数与作用域
来源：http://zb.muxihuayi.cn

================================================================================
来源：http://xq.huixinmuqiang.cn

[C01] 定义函数
来源：http://xf.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://nx.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vo.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://qu.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xe.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lt.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fe.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://pi.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://re.shxzukj.cn

[C02] 默认参数
来源：http://qv.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://na.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cd.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://oq.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wn.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kd.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ah.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://cq.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://gj.9csxet.cn

[C03] 可变参数
来源：http://ax.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://oo.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bd.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xk.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://we.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kt.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rd.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ud.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eq.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://fs.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ab.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tn.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vf.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sm.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://zc.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://xc.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://ip.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://xq.bjjhwx.cn

[C05] 返回多个值
来源：http://nt.chemitech.net.cn

Py:   return a, b
来源：http://cs.asd995.cn

PHP:  return [$a, $b];
来源：http://gy.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fr.haigaiapp.cn

TS:   return { a, b };
来源：http://em.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dp.szsharing.cn

Go:   return a, b
来源：http://ia.huixiangedu.cn

Ruby: return a, b
来源：http://en.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://us.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://co.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://nv.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wc.shxzskj.cn

JS:   const square = x => x * x;
来源：http://hs.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://qu.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dn.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://un.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ps.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cm.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://gj.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zs.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nd.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ff.shxzskj.cn

TS:   arr.map(String)
来源：http://fd.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ij.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gp.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://fz.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hn.yuntaijiaju.cn

[C08] 闭包
来源：http://dn.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mp.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gl.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kj.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zo.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://un.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mu.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zl.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://an.jctech888.com.cn

[C09] 递归
来源：http://iz.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gp.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nc.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fl.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jl.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rr.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://np.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fu.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ac.lnxyls.cn

[C10] 变量作用域
来源：http://ex.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ge.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pf.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gd.hahajie.cn

TS:   同 JS
来源：http://bm.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ls.panjiajie.cn

Go:   花括号块级作用域
来源：http://ly.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ny.nicolike.cn

C#:   块级作用域
来源：http://ez.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://ri.nicolike.cn

Py:   from module import func
来源：http://po.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kt.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ld.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rl.szxytkj.cn

Java: import java.util.List;
来源：http://ji.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bu.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ss.nszjky.cn

C#:   using System.Text;
来源：http://lz.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://wp.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://vg.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://qs.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://oh.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://yh.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tm.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://ed.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://nk.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vl.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://mo.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://on.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ee.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pq.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rg.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uf.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://za.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lm.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wn.chemitech.net.cn

[C14] 泛型函数
来源：http://co.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bh.lnxyls.cn

PHP:  // 无泛型
来源：http://tx.gzmigu.cn

JS:   // 无泛型
来源：http://jw.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://go.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jn.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lj.yuexingan06.cn

Ruby: # 无泛型
来源：http://ws.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fl.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://pb.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bu.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://za.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hx.newstarts.cn

Java: // 无解构
来源：http://ye.wgjwhj.cn

Go:   // 无解构
来源：http://yu.hahajie.cn

Ruby: a, b = pair
来源：http://ff.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://fs.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://eb.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cn.lnxyls.cn

PHP:  // 无重载
来源：http://px.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://to.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://vm.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gf.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://lj.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://vp.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iu.gzmigu.cn

================================================================================
来源：http://tf.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://zb.colortex.cn

================================================================================
来源：http://rg.colortex.cn

[D01] 创建数组 / 列表
来源：http://wu.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rm.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qd.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vc.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kf.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ts.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://ll.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://gr.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://rx.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://on.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rz.haigaiapp.cn

JS:   arr.push(4);
来源：http://yw.shxzskj.cn

TS:   arr.push(4);
来源：http://zd.521024.cn

Java: list.add(4);
来源：http://uy.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://yq.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ui.huanxung.cn

C#:   list.Add(4);
来源：http://fr.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://tx.521024.cn

Py:   arr.insert(0, 0)
来源：http://nx.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://la.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ro.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://cx.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://yw.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dz.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xz.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://kf.9csxet.cn

[D04] 删除元素
来源：http://zo.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cc.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ia.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ih.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://fr.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eg.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ck.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gx.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rg.huixiangedu.cn

[D05] 访问与修改元素
来源：http://no.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eu.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dk.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nz.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://ka.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://st.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xq.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dy.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dr.lnxyls.cn

[D06] 数组长度
来源：http://jx.shtwfgs.cn

Py:   len(arr)
来源：http://jx.shxzukj.cn

PHP:  count($arr);
来源：http://pi.shtwfgs.cn

JS:   arr.length
来源：http://dz.huixiangedu.cn

TS:   arr.length
来源：http://pa.yuntaijiaju.cn

Java: list.size();
来源：http://sz.shxzukj.cn

Go:   len(arr)
来源：http://jt.huanxung.cn

Ruby: arr.length; arr.size
来源：http://zc.hahajie.cn

C#:   list.Count;
来源：http://dz.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://fa.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ur.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ex.colortex.cn

JS:   arr.slice(1, 4);
来源：http://lb.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ke.521024.cn

Java: list.subList(1, 4);
来源：http://hu.colortex.cn

Go:   arr[1:4]
来源：http://sf.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://rx.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://xm.shtwfgs.cn

[D08] 合并两个数组
来源：http://ip.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://zy.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://yb.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wk.panjiajie.cn

TS:   [...a, ...b];
来源：http://zq.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yg.shtwfgs.cn

Go:   append(a, b...)
来源：http://kz.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://fu.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://bg.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://hi.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://qm.szxytkj.cn

PHP:  sort($arr);
来源：http://kz.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kf.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://on.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yd.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qz.yuexingan06.cn

Ruby: arr.sort
来源：http://zb.shxzukj.cn

C#:   list.Sort();
来源：http://dh.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ts.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iv.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gk.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cn.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://la.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rm.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ub.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jt.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pk.shtwfgs.cn

[D11] 反转数组
来源：http://hi.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hf.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://ha.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xn.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://yx.huanxung.cn

Java: Collections.reverse(list);
来源：http://mq.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://bb.huixiangedu.cn

Ruby: arr.reverse
来源：http://vh.huanxung.cn


<!-- 参考信息 -->