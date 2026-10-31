代发 wailian999

C#:   x is int or double or decimal
来源：http://jr.nicolike.cn

[B14] 判断值是否在集合内
来源：http://ji.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lw.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iq.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://aa.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ce.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ao.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gn.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kb.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://po.shxzukj.cn

Py:   a and b or not c
来源：http://ox.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://sd.gzmigu.cn

JS:   a && b || !c
来源：http://dp.chemitech.net.cn

TS:   a && b || !c
来源：http://rl.jianghongdianzi.cn

Java: a && b || !c
来源：http://gf.jctech888.com.cn

Go:   a && b || !c
来源：http://ft.hnjuh.cn

Ruby: a && b || !c
来源：http://ss.gzmigu.cn

C#:   a && b || !c
来源：http://fg.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bs.521024.cn

Py:   if not data: return
来源：http://nc.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://oe.szxytkj.cn

JS:   if (!data) return;
来源：http://dv.szsharing.cn

TS:   if (!data) return;
来源：http://rk.szsharing.cn

Java: if (data == null) return;
来源：http://th.lnxyls.cn

Go:   if data == nil { return }
来源：http://fd.muxihuayi.cn

Ruby: return if data.nil?
来源：http://gn.huanxung.cn

C#:   if (data == null) return;
来源：http://zg.521024.cn

================================================================================
来源：http://nm.nicolike.cn

C. 函数与作用域
来源：http://sx.huixinmuqiang.cn

================================================================================
来源：http://zm.asd995.cn

[C01] 定义函数
来源：http://bu.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://cl.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://co.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://gh.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wn.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nf.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jv.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://qs.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zq.jianghongdianzi.cn

[C02] 默认参数
来源：http://jy.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://pw.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vv.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://ub.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yt.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ij.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bt.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://mh.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://ao.shxzskj.cn

[C03] 可变参数
来源：http://xb.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://du.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sr.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rw.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bu.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bk.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ir.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tl.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ht.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ab.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ml.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ob.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hs.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qq.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ff.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://mg.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ds.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://bc.hahajie.cn

[C05] 返回多个值
来源：http://pb.haigaiapp.cn

Py:   return a, b
来源：http://fl.lnxyls.cn

PHP:  return [$a, $b];
来源：http://bk.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jv.hahajie.cn

TS:   return { a, b };
来源：http://an.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wc.jctech888.com.cn

Go:   return a, b
来源：http://pq.nicolike.cn

Ruby: return a, b
来源：http://xz.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://gb.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://so.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://kf.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dk.szsharing.cn

JS:   const square = x => x * x;
来源：http://yy.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sn.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://av.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dt.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://mr.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://go.hahajie.cn

[C07] 把函数作为参数传入
来源：http://bm.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nx.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://up.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lg.hahajie.cn

TS:   arr.map(String)
来源：http://tj.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vr.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cf.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://co.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cu.szxytkj.cn

[C08] 闭包
来源：http://qh.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bv.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rm.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wq.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vd.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iu.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tj.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rk.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ai.9csxet.cn

[C09] 递归
来源：http://rs.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gv.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hp.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lx.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://di.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://px.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uy.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jy.huixiangedu.cn

[C10] 变量作用域
来源：http://rh.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qh.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cf.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bu.hnjuh.cn

TS:   同 JS
来源：http://nk.panjiajie.cn

Java: 方法内为块级作用域
来源：http://qf.muxihuayi.cn

Go:   花括号块级作用域
来源：http://ys.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tx.nszjky.cn

C#:   块级作用域
来源：http://jb.hahajie.cn

[C11] 模块导入与导出
来源：http://mp.hnjuh.cn

Py:   from module import func
来源：http://jn.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gq.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ng.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nk.panjiajie.cn

Java: import java.util.List;
来源：http://ka.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aw.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://ab.shxzskj.cn

C#:   using System.Text;
来源：http://lm.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://sj.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://of.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://xp.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://gt.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://pr.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jq.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://dk.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://di.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://my.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ct.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xj.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ma.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fn.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ja.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bx.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://zn.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uv.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tc.nicolike.cn

[C14] 泛型函数
来源：http://pl.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gm.nszjky.cn

PHP:  // 无泛型
来源：http://ar.yuexingan06.cn

JS:   // 无泛型
来源：http://vz.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ja.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ok.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tz.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://aq.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fh.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://do.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://io.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://so.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dk.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jv.hahajie.cn

Java: // 无解构
来源：http://ja.haigaiapp.cn

Go:   // 无解构
来源：http://nb.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://zz.asd995.cn

C#:   var (a, b) = pair;
来源：http://ab.huanxung.cn

[C16] 函数 / 方法重载
来源：http://ke.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iu.huixiangedu.cn

PHP:  // 无重载
来源：http://as.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fz.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://bb.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yc.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ii.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://ob.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ga.szxytkj.cn

================================================================================
来源：http://yr.521024.cn

D. 数组 / 列表 / 集合
来源：http://cf.521024.cn

================================================================================
来源：http://gr.huanxung.cn

[D01] 创建数组 / 列表
来源：http://lp.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://an.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ya.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fx.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uj.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wt.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://xk.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://xs.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vx.9csxet.cn

[D02] 追加元素到末尾
来源：http://qw.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uc.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jc.panjiajie.cn

JS:   arr.push(4);
来源：http://tl.521024.cn

TS:   arr.push(4);
来源：http://wt.yuexingan06.cn

Java: list.add(4);
来源：http://xi.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://tx.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://yh.lnxyls.cn

C#:   list.Add(4);
来源：http://fp.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://ic.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://js.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dv.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xr.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://au.newstarts.cn

Java: list.add(0, 0);
来源：http://tk.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vo.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cl.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://mo.panjiajie.cn

[D04] 删除元素
来源：http://pu.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jq.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jb.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bs.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://ds.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kk.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qc.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hg.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uc.huixiangedu.cn

[D05] 访问与修改元素
来源：http://rf.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ha.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bs.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ra.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://nd.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://er.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://da.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sk.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ta.shxzukj.cn

[D06] 数组长度
来源：http://wo.hahajie.cn

Py:   len(arr)
来源：http://kx.nicolike.cn

PHP:  count($arr);
来源：http://kl.huanxung.cn

JS:   arr.length
来源：http://vi.9csxet.cn

TS:   arr.length
来源：http://kd.hnjuh.cn

Java: list.size();
来源：http://ja.asd995.cn

Go:   len(arr)
来源：http://kq.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://te.hahajie.cn

C#:   list.Count;
来源：http://mw.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://sf.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hv.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fw.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://lq.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ai.shxzskj.cn

Java: list.subList(1, 4);
来源：http://wa.asd995.cn

Go:   arr[1:4]
来源：http://cp.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://gh.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://tb.521024.cn

[D08] 合并两个数组
来源：http://oj.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://rf.asd995.cn

PHP:  array_merge($a, $b);
来源：http://co.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rp.newstarts.cn

TS:   [...a, ...b];
来源：http://ng.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sd.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://jm.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ws.521024.cn

C#:   a.Concat(b).ToList()
来源：http://it.jctech888.com.cn

[D09] 排序（升序）
来源：http://ab.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://gx.shxzskj.cn

PHP:  sort($arr);
来源：http://oa.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vn.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gt.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qk.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mj.huixiangedu.cn

Ruby: arr.sort
来源：http://av.hnjuh.cn

C#:   list.Sort();
来源：http://ad.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vg.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ef.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xf.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eq.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cp.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ll.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nh.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://si.huixiangedu.cn

[D11] 反转数组
来源：http://gl.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ww.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://fy.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nm.shxzukj.cn

TS:   [...arr].reverse();
来源：http://bj.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://zv.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://si.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ma.panjiajie.cn

C#:   list.Reverse();
来源：http://xc.haigaiapp.cn

[D12] 查找元素下标
来源：http://fh.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://uy.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xj.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pj.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://id.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://et.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://wh.jctech888.com.cn

Ruby: arr.index(x)
来源：http://xu.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://lz.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://cb.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://js.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://za.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://dv.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://yc.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rw.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zk.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uz.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://os.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://az.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ap.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nb.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://kv.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://gi.szxytkj.cn


<!-- 参考信息 -->