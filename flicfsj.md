代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://yy.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kg.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gc.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dt.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gu.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ub.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zx.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mc.colortex.cn

[B13] 判断是否为数字
来源：http://mj.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://yy.szsharing.cn

PHP:  is_numeric($x)
来源：http://hl.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ox.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lu.panjiajie.cn

Java: x instanceof Number
来源：http://ct.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bu.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://cu.gzmigu.cn

C#:   x is int or double or decimal
来源：http://ip.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://ap.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qr.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fr.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://hl.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://mc.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rr.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tu.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://em.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pd.gzmigu.cn

[B15] 布尔运算与取反
来源：http://xw.colortex.cn

Py:   a and b or not c
来源：http://vi.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://wd.nicolike.cn

JS:   a && b || !c
来源：http://jo.szsharing.cn

TS:   a && b || !c
来源：http://tv.yuexingan06.cn

Java: a && b || !c
来源：http://sv.huixiangedu.cn

Go:   a && b || !c
来源：http://mk.newstarts.cn

Ruby: a && b || !c
来源：http://jq.chemitech.net.cn

C#:   a && b || !c
来源：http://go.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lm.521024.cn

Py:   if not data: return
来源：http://ht.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://zs.colortex.cn

JS:   if (!data) return;
来源：http://wi.shxzskj.cn

TS:   if (!data) return;
来源：http://op.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://kn.panjiajie.cn

Go:   if data == nil { return }
来源：http://gt.bjjhwx.cn

Ruby: return if data.nil?
来源：http://hx.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://rl.shtwfgs.cn

================================================================================
来源：http://dx.jianghongdianzi.cn

C. 函数与作用域
来源：http://go.huanxung.cn

================================================================================
来源：http://bo.shxzskj.cn

[C01] 定义函数
来源：http://pq.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://di.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gh.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://jo.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ae.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pm.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xf.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://ql.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rv.panjiajie.cn

[C02] 默认参数
来源：http://cu.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://xy.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vv.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://qc.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://th.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rd.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://oq.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ao.shxzukj.cn

[C03] 可变参数
来源：http://hk.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://oy.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dk.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vh.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://df.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cq.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ah.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hk.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oq.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://si.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sb.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fm.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cs.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://to.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zg.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://va.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://zf.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://lg.jctech888.com.cn

[C05] 返回多个值
来源：http://cg.newstarts.cn

Py:   return a, b
来源：http://uy.nszjky.cn

PHP:  return [$a, $b];
来源：http://ka.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dt.bjjhwx.cn

TS:   return { a, b };
来源：http://gg.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://db.9csxet.cn

Go:   return a, b
来源：http://hi.9csxet.cn

Ruby: return a, b
来源：http://cg.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://qk.asd995.cn

[C06] 匿名函数 / lambda
来源：http://lz.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://gs.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qq.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://up.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://in.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bw.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://au.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://oy.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nd.asd995.cn

[C07] 把函数作为参数传入
来源：http://wu.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xv.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uu.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sb.521024.cn

TS:   arr.map(String)
来源：http://en.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ob.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gk.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://nb.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dt.yuntaijiaju.cn

[C08] 闭包
来源：http://ab.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jx.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yg.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nx.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mq.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jo.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hv.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eb.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rs.newstarts.cn

[C09] 递归
来源：http://bo.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://va.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tc.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nr.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wt.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ti.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bk.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rn.huanxung.cn

[C10] 变量作用域
来源：http://wy.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wx.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ge.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nm.asd995.cn

TS:   同 JS
来源：http://md.gzmigu.cn

Java: 方法内为块级作用域
来源：http://cq.wgjwhj.cn

Go:   花括号块级作用域
来源：http://id.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yl.nszjky.cn

C#:   块级作用域
来源：http://ei.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://ou.huixiangedu.cn

Py:   from module import func
来源：http://nu.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rc.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zp.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tb.nicolike.cn

Java: import java.util.List;
来源：http://sn.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cs.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://kv.bookmarksfly.cn

C#:   using System.Text;
来源：http://gk.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://za.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://of.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://ty.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://hv.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://cx.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bw.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://qh.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://eh.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wo.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://es.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sl.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qe.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ah.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fn.nszjky.cn

Go:   func add(a, b int) int
来源：http://bm.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://go.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ti.yuexingan06.cn

[C14] 泛型函数
来源：http://zl.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://va.asd995.cn

PHP:  // 无泛型
来源：http://ki.gzmigu.cn

JS:   // 无泛型
来源：http://jr.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yr.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://po.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pv.wgjwhj.cn

Ruby: # 无泛型
来源：http://yb.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kz.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://hm.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oo.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://ts.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jl.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ln.jianghongdianzi.cn

Java: // 无解构
来源：http://ab.jctech888.com.cn

Go:   // 无解构
来源：http://do.huanxung.cn

Ruby: a, b = pair
来源：http://dv.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://of.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ej.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://op.hnjuh.cn

PHP:  // 无重载
来源：http://zw.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ls.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ij.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pg.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://az.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://td.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rf.gzmigu.cn

================================================================================
来源：http://nz.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://zc.lnxyls.cn

================================================================================
来源：http://xd.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://da.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://it.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ud.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wm.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ze.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xw.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://xg.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://rq.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gn.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://gp.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vz.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fd.colortex.cn

JS:   arr.push(4);
来源：http://nm.haigaiapp.cn

TS:   arr.push(4);
来源：http://cf.haigaiapp.cn

Java: list.add(4);
来源：http://ed.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://av.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://jz.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://zx.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://rt.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://ts.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jb.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jf.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://xa.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://fy.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oe.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ud.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://il.wgjwhj.cn

[D04] 删除元素
来源：http://qp.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tv.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pc.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vk.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://hl.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pd.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hn.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kx.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ja.huixiangedu.cn

[D05] 访问与修改元素
来源：http://yw.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xj.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zj.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mc.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://hv.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://am.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://zg.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jq.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yv.jianghongdianzi.cn

[D06] 数组长度
来源：http://md.hnjuh.cn

Py:   len(arr)
来源：http://fd.chemitech.net.cn

PHP:  count($arr);
来源：http://fb.hahajie.cn

JS:   arr.length
来源：http://fs.asd995.cn

TS:   arr.length
来源：http://vc.asd995.cn

Java: list.size();
来源：http://gt.chemitech.net.cn

Go:   len(arr)
来源：http://nh.521024.cn

Ruby: arr.length; arr.size
来源：http://xr.gzmigu.cn

C#:   list.Count;
来源：http://br.szsharing.cn

[D07] 切片 / 取子数组
来源：http://ct.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rj.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vn.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://kr.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://xg.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://cs.lnxyls.cn

Go:   arr[1:4]
来源：http://zu.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://yy.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://hf.shtwfgs.cn

[D08] 合并两个数组
来源：http://xy.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://nt.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://tu.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qn.huanxung.cn

TS:   [...a, ...b];
来源：http://lh.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lj.shxzskj.cn

Go:   append(a, b...)
来源：http://rh.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://gn.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://at.shxzukj.cn

[D09] 排序（升序）
来源：http://ea.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://re.panjiajie.cn

PHP:  sort($arr);
来源：http://ei.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xk.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fx.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oy.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://om.panjiajie.cn

Ruby: arr.sort
来源：http://qo.hahajie.cn

C#:   list.Sort();
来源：http://bl.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ee.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nb.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yt.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jq.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lp.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pz.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eh.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wy.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mr.chemitech.net.cn

[D11] 反转数组
来源：http://ze.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xb.nszjky.cn

PHP:  array_reverse($arr);
来源：http://ay.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oc.nicolike.cn

TS:   [...arr].reverse();
来源：http://ld.9csxet.cn

Java: Collections.reverse(list);
来源：http://mk.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://rg.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://yj.bookmarksfly.cn

C#:   list.Reverse();
来源：http://yn.newstarts.cn

[D12] 查找元素下标
来源：http://kb.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://cj.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rh.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ib.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mm.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ln.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://em.jianghongdianzi.cn


<!-- 参考信息 -->