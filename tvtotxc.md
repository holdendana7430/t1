代发 wailian999

[B13] 判断是否为数字
来源：http://gw.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://ox.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://hz.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ws.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://im.szxytkj.cn

Java: x instanceof Number
来源：http://eo.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tj.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://tt.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ud.nicolike.cn

[B14] 判断值是否在集合内
来源：http://pa.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gi.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zm.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ah.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://aw.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bx.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yq.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cu.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://id.huanxung.cn

[B15] 布尔运算与取反
来源：http://ja.hnjuh.cn

Py:   a and b or not c
来源：http://uk.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://bm.huixiangedu.cn

JS:   a && b || !c
来源：http://fa.jianghongdianzi.cn

TS:   a && b || !c
来源：http://bx.hnjuh.cn

Java: a && b || !c
来源：http://sa.yuexingan06.cn

Go:   a && b || !c
来源：http://et.chemitech.net.cn

Ruby: a && b || !c
来源：http://oq.huanxung.cn

C#:   a && b || !c
来源：http://pi.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://di.asd995.cn

Py:   if not data: return
来源：http://wb.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://xb.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ma.jctech888.com.cn

TS:   if (!data) return;
来源：http://pp.shxzukj.cn

Java: if (data == null) return;
来源：http://vi.nicolike.cn

Go:   if data == nil { return }
来源：http://ha.panjiajie.cn

Ruby: return if data.nil?
来源：http://hl.hahajie.cn

C#:   if (data == null) return;
来源：http://oi.gzmigu.cn

================================================================================
来源：http://ux.chemitech.net.cn

C. 函数与作用域
来源：http://qr.521024.cn

================================================================================
来源：http://bp.yuntaijiaju.cn

[C01] 定义函数
来源：http://ty.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://hy.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iu.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://wr.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ag.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fz.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ia.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://st.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://en.huixiangedu.cn

[C02] 默认参数
来源：http://hh.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://rj.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kw.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://rh.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rn.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://et.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gq.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://tu.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://uv.chemitech.net.cn

[C03] 可变参数
来源：http://al.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://rj.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xw.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dw.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ro.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://st.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ae.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lj.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://et.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://rs.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ko.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ji.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qr.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wk.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://mq.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://oc.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://zu.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://hr.shxzskj.cn

[C05] 返回多个值
来源：http://gj.huanxung.cn

Py:   return a, b
来源：http://wa.lnxyls.cn

PHP:  return [$a, $b];
来源：http://vi.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mj.panjiajie.cn

TS:   return { a, b };
来源：http://xh.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qm.nszjky.cn

Go:   return a, b
来源：http://nm.panjiajie.cn

Ruby: return a, b
来源：http://up.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://ly.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://cc.asd995.cn

Py:   square = lambda x: x * x
来源：http://kb.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kl.shxzskj.cn

JS:   const square = x => x * x;
来源：http://yn.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sg.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bf.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bc.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://gr.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zi.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://qv.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jv.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iz.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vq.muxihuayi.cn

TS:   arr.map(String)
来源：http://oq.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kc.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://as.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://yo.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sy.asd995.cn

[C08] 闭包
来源：http://fp.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://us.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xy.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lk.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yv.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://py.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tg.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ri.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tw.jctech888.com.cn

[C09] 递归
来源：http://dz.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xq.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://da.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yn.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wg.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rb.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mi.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yo.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gg.yuexingan06.cn

[C10] 变量作用域
来源：http://ur.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bg.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cl.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://es.shxzukj.cn

TS:   同 JS
来源：http://ib.szsharing.cn

Java: 方法内为块级作用域
来源：http://kq.haigaiapp.cn

Go:   花括号块级作用域
来源：http://zj.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dc.bjjhwx.cn

C#:   块级作用域
来源：http://li.panjiajie.cn

[C11] 模块导入与导出
来源：http://cd.chemitech.net.cn

Py:   from module import func
来源：http://ld.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://np.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ng.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zl.yuntaijiaju.cn

Java: import java.util.List;
来源：http://tt.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nb.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://as.huixiangedu.cn

C#:   using System.Text;
来源：http://fd.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://qo.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://bi.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://fi.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://pv.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://da.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gr.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://gf.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://mq.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ub.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://li.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://al.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oc.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tx.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rt.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bv.shxzskj.cn

Go:   func add(a, b int) int
来源：http://yv.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wd.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fh.lnxyls.cn

[C14] 泛型函数
来源：http://ju.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mk.jctech888.com.cn

PHP:  // 无泛型
来源：http://gp.huanxung.cn

JS:   // 无泛型
来源：http://xe.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://za.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://le.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dv.nszjky.cn

Ruby: # 无泛型
来源：http://ul.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xl.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://ag.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sf.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://yi.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xu.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://so.shxzukj.cn

Java: // 无解构
来源：http://iz.asd995.cn

Go:   // 无解构
来源：http://gn.wgjwhj.cn

Ruby: a, b = pair
来源：http://eg.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://fz.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ve.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zf.hahajie.cn

PHP:  // 无重载
来源：http://up.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jr.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://cd.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qf.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://me.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://tr.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ws.panjiajie.cn

================================================================================
来源：http://um.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://mh.asd995.cn

================================================================================
来源：http://wq.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ap.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jd.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ua.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gy.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hs.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pm.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://cl.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://pi.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://km.hnjuh.cn

[D02] 追加元素到末尾
来源：http://ui.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zg.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://co.szxytkj.cn

JS:   arr.push(4);
来源：http://gb.nszjky.cn

TS:   arr.push(4);
来源：http://ip.9csxet.cn

Java: list.add(4);
来源：http://cg.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://jx.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://sh.hnjuh.cn

C#:   list.Add(4);
来源：http://zo.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://jz.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://hv.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qb.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ky.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://mu.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://ku.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lq.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yy.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://fr.newstarts.cn

[D04] 删除元素
来源：http://gj.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mj.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vk.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xl.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://mo.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gz.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qv.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ef.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sn.shxzukj.cn

[D05] 访问与修改元素
来源：http://hh.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zp.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ud.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wb.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://kh.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://wi.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://ba.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://an.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gu.yuntaijiaju.cn

[D06] 数组长度
来源：http://zu.gzmigu.cn

Py:   len(arr)
来源：http://in.521024.cn

PHP:  count($arr);
来源：http://ua.muxihuayi.cn

JS:   arr.length
来源：http://xr.yuntaijiaju.cn

TS:   arr.length
来源：http://vx.nszjky.cn

Java: list.size();
来源：http://mh.bookmarksfly.cn

Go:   len(arr)
来源：http://fw.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://ju.huixinmuqiang.cn

C#:   list.Count;
来源：http://qw.nszjky.cn

[D07] 切片 / 取子数组
来源：http://oo.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vs.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tc.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://rd.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://bo.szsharing.cn

Java: list.subList(1, 4);
来源：http://mn.gzmigu.cn

Go:   arr[1:4]
来源：http://fo.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://ey.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://or.wgjwhj.cn

[D08] 合并两个数组
来源：http://te.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://ds.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://ws.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lz.huanxung.cn

TS:   [...a, ...b];
来源：http://eg.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rc.bookmarksfly.cn

Go:   append(a, b...)
来源：http://go.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://jf.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://nw.szsharing.cn

[D09] 排序（升序）
来源：http://ft.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://bf.nszjky.cn

PHP:  sort($arr);
来源：http://oy.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pd.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bd.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lw.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lk.hnjuh.cn

Ruby: arr.sort
来源：http://oc.hahajie.cn

C#:   list.Sort();
来源：http://ux.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mw.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://og.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gi.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iy.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://df.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ln.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xf.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xz.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mt.shxzskj.cn

[D11] 反转数组
来源：http://ov.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ol.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://cy.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xf.shxzukj.cn

TS:   [...arr].reverse();
来源：http://ts.gzmigu.cn

Java: Collections.reverse(list);
来源：http://lu.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://ce.szsharing.cn

Ruby: arr.reverse
来源：http://me.nszjky.cn

C#:   list.Reverse();
来源：http://kl.muxihuayi.cn

[D12] 查找元素下标
来源：http://ho.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://by.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://um.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ij.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rq.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://br.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://xf.hahajie.cn

Ruby: arr.index(x)
来源：http://ud.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://wu.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://mc.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yb.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xd.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://id.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://gp.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://no.hahajie.cn


<!-- 参考信息 -->