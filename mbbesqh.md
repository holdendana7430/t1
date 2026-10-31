代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yc.szxytkj.cn

Java: x instanceof Number
来源：http://sf.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pa.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://rw.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://wn.newstarts.cn

[B14] 判断值是否在集合内
来源：http://lo.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gn.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pt.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://hb.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ny.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ii.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bi.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ci.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vd.huanxung.cn

[B15] 布尔运算与取反
来源：http://bg.panjiajie.cn

Py:   a and b or not c
来源：http://xm.hahajie.cn

PHP:  $a && $b || !$c
来源：http://ak.haigaiapp.cn

JS:   a && b || !c
来源：http://tw.muxihuayi.cn

TS:   a && b || !c
来源：http://nk.yuntaijiaju.cn

Java: a && b || !c
来源：http://wi.hahajie.cn

Go:   a && b || !c
来源：http://eu.panjiajie.cn

Ruby: a && b || !c
来源：http://or.colortex.cn

C#:   a && b || !c
来源：http://be.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bv.huixinmuqiang.cn

Py:   if not data: return
来源：http://qx.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://uq.huanxung.cn

JS:   if (!data) return;
来源：http://ff.panjiajie.cn

TS:   if (!data) return;
来源：http://hd.bjjhwx.cn

Java: if (data == null) return;
来源：http://ut.yuexingan06.cn

Go:   if data == nil { return }
来源：http://ul.hahajie.cn

Ruby: return if data.nil?
来源：http://sc.szsharing.cn

C#:   if (data == null) return;
来源：http://tk.bjjhwx.cn

================================================================================
来源：http://sn.newstarts.cn

C. 函数与作用域
来源：http://uf.huanxung.cn

================================================================================
来源：http://ke.shtwfgs.cn

[C01] 定义函数
来源：http://ij.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://qw.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jv.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://gr.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qr.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ga.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ox.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://ht.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://li.nicolike.cn

[C02] 默认参数
来源：http://wj.asd995.cn

Py:   def greet(name="World"): return name
来源：http://jy.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jy.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://eo.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pr.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fx.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uz.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://fy.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://bq.haigaiapp.cn

[C03] 可变参数
来源：http://zf.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://xy.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xg.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ta.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gn.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wn.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xs.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yp.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ub.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kk.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jb.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://re.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mk.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://mc.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://lg.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://hz.bjjhwx.cn

[C05] 返回多个值
来源：http://ve.yuntaijiaju.cn

Py:   return a, b
来源：http://sq.szsharing.cn

PHP:  return [$a, $b];
来源：http://wd.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ow.huanxung.cn

TS:   return { a, b };
来源：http://uk.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sf.haigaiapp.cn

Go:   return a, b
来源：http://ay.huixiangedu.cn

Ruby: return a, b
来源：http://zu.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://cf.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://dm.colortex.cn

Py:   square = lambda x: x * x
来源：http://cx.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.colortex.cn

JS:   const square = x => x * x;
来源：http://cg.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://yg.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ex.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fc.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://jd.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jz.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://eb.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bn.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://br.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gv.yuexingan06.cn

TS:   arr.map(String)
来源：http://hi.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hm.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ir.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://xm.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://am.yuexingan06.cn

[C08] 闭包
来源：http://cc.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zy.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ci.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jr.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wa.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qa.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cj.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cz.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bk.gzmigu.cn

[C09] 递归
来源：http://zu.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oz.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cf.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://al.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sq.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pw.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zf.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xe.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mu.bjjhwx.cn

[C10] 变量作用域
来源：http://uf.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xr.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://us.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zh.szxytkj.cn

TS:   同 JS
来源：http://rg.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ta.wgjwhj.cn

Go:   花括号块级作用域
来源：http://mb.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ix.huixiangedu.cn

C#:   块级作用域
来源：http://xs.yuexingan06.cn

[C11] 模块导入与导出
来源：http://vk.jianghongdianzi.cn

Py:   from module import func
来源：http://if.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ra.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zk.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cy.yuexingan06.cn

Java: import java.util.List;
来源：http://lr.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vq.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://jj.gzmigu.cn

C#:   using System.Text;
来源：http://ls.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://yn.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://ck.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://xf.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://jv.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://yd.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zp.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ym.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://tx.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ro.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://rs.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yf.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rq.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bs.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lo.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uo.colortex.cn

Go:   func add(a, b int) int
来源：http://qq.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qo.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sj.jctech888.com.cn

[C14] 泛型函数
来源：http://hs.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nx.bookmarksfly.cn

PHP:  // 无泛型
来源：http://xj.shtwfgs.cn

JS:   // 无泛型
来源：http://hq.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bd.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rr.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qr.nszjky.cn

Ruby: # 无泛型
来源：http://qb.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bs.hahajie.cn

[C15] 解构 / 展开参数
来源：http://kq.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ip.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://eu.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ti.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uc.lnxyls.cn

Java: // 无解构
来源：http://gz.521024.cn

Go:   // 无解构
来源：http://zf.521024.cn

Ruby: a, b = pair
来源：http://xz.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://ck.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://jx.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ar.wgjwhj.cn

PHP:  // 无重载
来源：http://kv.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cf.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://rp.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ts.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://gc.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://tz.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://se.szxytkj.cn

================================================================================
来源：http://kf.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://es.huixinmuqiang.cn

================================================================================
来源：http://rb.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://cd.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fg.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ww.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ck.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yj.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fe.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://oh.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://dg.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sn.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://yt.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bu.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yw.newstarts.cn

JS:   arr.push(4);
来源：http://hg.colortex.cn

TS:   arr.push(4);
来源：http://sj.gzmigu.cn

Java: list.add(4);
来源：http://da.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://iu.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://av.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://kj.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://vu.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://of.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dx.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yt.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://cj.nicolike.cn

Java: list.add(0, 0);
来源：http://by.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rl.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dw.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://im.shxzukj.cn

[D04] 删除元素
来源：http://lz.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zo.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://so.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://az.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://vg.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ed.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tu.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tk.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pn.lnxyls.cn

[D05] 访问与修改元素
来源：http://xs.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qd.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ig.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://po.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://la.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://mk.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://mu.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vt.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xx.szsharing.cn

[D06] 数组长度
来源：http://uh.yuexingan06.cn

Py:   len(arr)
来源：http://yy.shtwfgs.cn

PHP:  count($arr);
来源：http://ol.521024.cn

JS:   arr.length
来源：http://fu.hahajie.cn

TS:   arr.length
来源：http://hz.huixiangedu.cn

Java: list.size();
来源：http://hp.asd995.cn

Go:   len(arr)
来源：http://sc.9csxet.cn

Ruby: arr.length; arr.size
来源：http://uf.lnxyls.cn

C#:   list.Count;
来源：http://uj.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ka.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lb.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qa.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://sg.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://bv.hnjuh.cn

Java: list.subList(1, 4);
来源：http://yt.shxzukj.cn

Go:   arr[1:4]
来源：http://hj.huanxung.cn

Ruby: arr[1, 3]
来源：http://xa.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://eq.nszjky.cn

[D08] 合并两个数组
来源：http://wr.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://gd.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ao.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://le.shtwfgs.cn

TS:   [...a, ...b];
来源：http://qa.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xm.gzmigu.cn

Go:   append(a, b...)
来源：http://mg.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://uy.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://dm.shtwfgs.cn

[D09] 排序（升序）
来源：http://zv.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://od.hahajie.cn

PHP:  sort($arr);
来源：http://js.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mc.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cu.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ch.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zz.huixiangedu.cn

Ruby: arr.sort
来源：http://nm.bookmarksfly.cn

C#:   list.Sort();
来源：http://kb.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rq.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ka.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hw.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ht.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nd.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://in.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kl.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ni.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pj.yuntaijiaju.cn

[D11] 反转数组
来源：http://wu.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cn.colortex.cn

PHP:  array_reverse($arr);
来源：http://aa.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qk.huanxung.cn

TS:   [...arr].reverse();
来源：http://so.hahajie.cn

Java: Collections.reverse(list);
来源：http://ct.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://sr.newstarts.cn

Ruby: arr.reverse
来源：http://nm.asd995.cn

C#:   list.Reverse();
来源：http://wc.521024.cn

[D12] 查找元素下标
来源：http://ux.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://vk.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eq.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nh.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jk.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mz.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://eu.panjiajie.cn

Ruby: arr.index(x)
来源：http://rb.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://yr.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://xn.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cr.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sk.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://cf.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://bb.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qh.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ub.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://br.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bp.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://oo.hahajie.cn


<!-- 参考信息 -->