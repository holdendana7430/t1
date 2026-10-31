代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bv.panjiajie.cn

Java: x instanceof Number
来源：http://nv.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ki.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://vb.szxytkj.cn

C#:   x is int or double or decimal
来源：http://da.szsharing.cn

[B14] 判断值是否在集合内
来源：http://yr.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vv.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ib.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://qg.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://uh.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hh.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hc.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ws.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sz.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://jn.shxzskj.cn

Py:   a and b or not c
来源：http://wp.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://me.shxzukj.cn

JS:   a && b || !c
来源：http://dm.wgjwhj.cn

TS:   a && b || !c
来源：http://xz.colortex.cn

Java: a && b || !c
来源：http://yu.bjjhwx.cn

Go:   a && b || !c
来源：http://mi.szxytkj.cn

Ruby: a && b || !c
来源：http://gm.jianghongdianzi.cn

C#:   a && b || !c
来源：http://pz.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hl.shtwfgs.cn

Py:   if not data: return
来源：http://we.asd995.cn

PHP:  if (!$data) { return; }
来源：http://hn.shxzukj.cn

JS:   if (!data) return;
来源：http://ol.panjiajie.cn

TS:   if (!data) return;
来源：http://yt.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://rx.shtwfgs.cn

Go:   if data == nil { return }
来源：http://is.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://vj.gzmigu.cn

C#:   if (data == null) return;
来源：http://sx.yuexingan06.cn

================================================================================
来源：http://lx.yuexingan06.cn

C. 函数与作用域
来源：http://zq.huixiangedu.cn

================================================================================
来源：http://bh.bjjhwx.cn

[C01] 定义函数
来源：http://nb.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ci.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://os.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://vs.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rj.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rh.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ne.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://xd.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://or.lnxyls.cn

[C02] 默认参数
来源：http://zz.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ea.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vw.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://ld.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ly.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tv.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fd.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://zy.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://dw.bjjhwx.cn

[C03] 可变参数
来源：http://mu.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ka.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ak.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rd.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fo.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dt.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pf.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://el.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://th.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://sa.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zz.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iw.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aa.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://en.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://qp.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ke.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://fv.colortex.cn

[C05] 返回多个值
来源：http://wh.colortex.cn

Py:   return a, b
来源：http://wg.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://hs.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ap.nicolike.cn

TS:   return { a, b };
来源：http://hc.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ap.huixiangedu.cn

Go:   return a, b
来源：http://va.521024.cn

Ruby: return a, b
来源：http://aq.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://my.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://gf.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://km.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qk.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://bu.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://qw.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ri.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ff.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://lz.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://az.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://bj.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pz.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mj.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nu.shxzukj.cn

TS:   arr.map(String)
来源：http://md.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xn.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ro.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://pi.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ni.bookmarksfly.cn

[C08] 闭包
来源：http://ja.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vx.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ap.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iu.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tu.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bf.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uo.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bb.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ha.wgjwhj.cn

[C09] 递归
来源：http://ww.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eo.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dr.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yf.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dh.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oz.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bw.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://av.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oh.muxihuayi.cn

[C10] 变量作用域
来源：http://hh.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ie.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rj.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wl.yuexingan06.cn

TS:   同 JS
来源：http://kr.colortex.cn

Java: 方法内为块级作用域
来源：http://hd.shtwfgs.cn

Go:   花括号块级作用域
来源：http://jo.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fi.asd995.cn

C#:   块级作用域
来源：http://na.9csxet.cn

[C11] 模块导入与导出
来源：http://xz.hahajie.cn

Py:   from module import func
来源：http://jc.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jw.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uy.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tj.nszjky.cn

Java: import java.util.List;
来源：http://oc.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mu.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://fh.bjjhwx.cn

C#:   using System.Text;
来源：http://tw.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://wh.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://gg.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://wj.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://to.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ue.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yb.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://bs.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://jx.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://os.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ig.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wz.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gw.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://to.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jg.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mw.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://jo.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ul.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eh.muxihuayi.cn

[C14] 泛型函数
来源：http://um.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uy.hahajie.cn

PHP:  // 无泛型
来源：http://uj.jianghongdianzi.cn

JS:   // 无泛型
来源：http://xp.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iw.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tg.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wa.shtwfgs.cn

Ruby: # 无泛型
来源：http://cp.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wp.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://wi.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sh.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://yl.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yp.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ui.colortex.cn

Java: // 无解构
来源：http://eu.9csxet.cn

Go:   // 无解构
来源：http://rs.huanxung.cn

Ruby: a, b = pair
来源：http://ra.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://uw.newstarts.cn

[C16] 函数 / 方法重载
来源：http://za.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://su.521024.cn

PHP:  // 无重载
来源：http://gx.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pq.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gi.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cu.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://dw.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://nc.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xw.lnxyls.cn

================================================================================
来源：http://nv.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://ld.gzmigu.cn

================================================================================
来源：http://gt.nszjky.cn

[D01] 创建数组 / 列表
来源：http://qk.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qp.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://py.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sj.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vx.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bq.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://nj.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://wo.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hc.hahajie.cn

[D02] 追加元素到末尾
来源：http://fq.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yb.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hs.bjjhwx.cn

JS:   arr.push(4);
来源：http://eq.bjjhwx.cn

TS:   arr.push(4);
来源：http://jt.bookmarksfly.cn

Java: list.add(4);
来源：http://nk.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://mf.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://qu.muxihuayi.cn

C#:   list.Add(4);
来源：http://pk.colortex.cn

[D03] 在指定位置插入元素
来源：http://ge.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://hc.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tc.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bx.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://mr.lnxyls.cn

Java: list.add(0, 0);
来源：http://gh.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vb.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mf.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://ec.muxihuayi.cn

[D04] 删除元素
来源：http://ft.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aa.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zk.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xp.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://cu.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://as.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mi.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lr.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ve.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ml.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sy.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zw.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tb.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://dq.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://pr.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://kk.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mw.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kk.muxihuayi.cn

[D06] 数组长度
来源：http://hk.shtwfgs.cn

Py:   len(arr)
来源：http://za.szsharing.cn

PHP:  count($arr);
来源：http://ym.jctech888.com.cn

JS:   arr.length
来源：http://iz.asd995.cn

TS:   arr.length
来源：http://qo.nszjky.cn

Java: list.size();
来源：http://gk.muxihuayi.cn

Go:   len(arr)
来源：http://xw.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ob.newstarts.cn

C#:   list.Count;
来源：http://fo.newstarts.cn

[D07] 切片 / 取子数组
来源：http://am.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zh.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mh.asd995.cn

JS:   arr.slice(1, 4);
来源：http://ot.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://fg.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://ip.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://rj.gzmigu.cn

Ruby: arr[1, 3]
来源：http://cs.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://kt.haigaiapp.cn

[D08] 合并两个数组
来源：http://od.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://xh.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ie.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hn.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://uh.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gs.hahajie.cn

Go:   append(a, b...)
来源：http://ux.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://xk.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://up.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://to.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yi.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://yg.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vj.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zx.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rh.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ms.hnjuh.cn

Ruby: arr.sort
来源：http://ae.yuntaijiaju.cn

C#:   list.Sort();
来源：http://mu.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ah.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qi.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yn.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://as.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ld.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bh.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pu.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ij.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fv.bjjhwx.cn

[D11] 反转数组
来源：http://na.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ex.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://wk.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dl.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://vp.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://uq.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://go.hahajie.cn

Ruby: arr.reverse
来源：http://rk.shxzskj.cn

C#:   list.Reverse();
来源：http://jl.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://mf.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://xg.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gj.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xx.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zy.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gv.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ar.bjjhwx.cn

Ruby: arr.index(x)
来源：http://so.asd995.cn

C#:   list.IndexOf(x);
来源：http://jd.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://rv.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mt.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rx.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://xe.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://hg.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nq.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://an.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ty.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ux.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://dn.wgjwhj.cn


<!-- 参考信息 -->