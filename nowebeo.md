代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://ti.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://fe.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lt.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kf.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://gk.shtwfgs.cn

Py:   a and b or not c
来源：http://xp.newstarts.cn

PHP:  $a && $b || !$c
来源：http://vc.szxytkj.cn

JS:   a && b || !c
来源：http://nx.haigaiapp.cn

TS:   a && b || !c
来源：http://mn.szsharing.cn

Java: a && b || !c
来源：http://fd.yuexingan06.cn

Go:   a && b || !c
来源：http://tj.shxzskj.cn

Ruby: a && b || !c
来源：http://du.huixiangedu.cn

C#:   a && b || !c
来源：http://av.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bd.nszjky.cn

Py:   if not data: return
来源：http://ao.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://rf.colortex.cn

JS:   if (!data) return;
来源：http://jf.panjiajie.cn

TS:   if (!data) return;
来源：http://ca.huanxung.cn

Java: if (data == null) return;
来源：http://jt.newstarts.cn

Go:   if data == nil { return }
来源：http://kw.szxytkj.cn

Ruby: return if data.nil?
来源：http://tv.hnjuh.cn

C#:   if (data == null) return;
来源：http://kr.jctech888.com.cn

================================================================================
来源：http://wd.colortex.cn

C. 函数与作用域
来源：http://qi.huanxung.cn

================================================================================
来源：http://wo.asd995.cn

[C01] 定义函数
来源：http://ie.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://rs.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://av.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://iu.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qu.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ba.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://db.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://kh.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cj.hahajie.cn

[C02] 默认参数
来源：http://fg.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://zi.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fi.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://za.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ve.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bg.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://au.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://bq.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://he.muxihuayi.cn

[C03] 可变参数
来源：http://lg.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ki.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kt.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zu.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://no.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rn.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rv.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bi.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gb.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://gx.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bc.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cu.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ti.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oj.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://uz.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://uy.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://rt.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://qc.jctech888.com.cn

[C05] 返回多个值
来源：http://mj.newstarts.cn

Py:   return a, b
来源：http://dz.nszjky.cn

PHP:  return [$a, $b];
来源：http://qh.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://is.colortex.cn

TS:   return { a, b };
来源：http://wr.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bf.nszjky.cn

Go:   return a, b
来源：http://ll.haigaiapp.cn

Ruby: return a, b
来源：http://bb.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://gl.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://nf.colortex.cn

Py:   square = lambda x: x * x
来源：http://zk.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sp.gzmigu.cn

JS:   const square = x => x * x;
来源：http://vl.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://vk.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kp.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sb.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://wa.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xb.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://dn.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qk.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vf.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ni.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://ok.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dp.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fw.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://dn.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vd.yuexingan06.cn

[C08] 闭包
来源：http://fy.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uj.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://py.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ay.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bh.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wy.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://my.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rd.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ln.panjiajie.cn

[C09] 递归
来源：http://oz.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xt.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ul.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kk.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ev.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jd.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pr.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uk.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vh.jctech888.com.cn

[C10] 变量作用域
来源：http://mq.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lm.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jd.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vl.asd995.cn

TS:   同 JS
来源：http://kh.521024.cn

Java: 方法内为块级作用域
来源：http://tl.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://fc.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zr.newstarts.cn

C#:   块级作用域
来源：http://dc.hnjuh.cn

[C11] 模块导入与导出
来源：http://ot.521024.cn

Py:   from module import func
来源：http://mk.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nn.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bi.gzmigu.cn

Java: import java.util.List;
来源：http://cl.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ow.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://zz.9csxet.cn

C#:   using System.Text;
来源：http://ib.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://on.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://yq.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://ln.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://nv.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://gc.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ln.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://tb.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://bu.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yo.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://pi.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cl.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://in.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jn.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gg.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vf.gzmigu.cn

Go:   func add(a, b int) int
来源：http://lh.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rk.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vt.chemitech.net.cn

[C14] 泛型函数
来源：http://al.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fu.haigaiapp.cn

PHP:  // 无泛型
来源：http://ox.muxihuayi.cn

JS:   // 无泛型
来源：http://oa.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tm.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ks.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://am.shxzukj.cn

Ruby: # 无泛型
来源：http://kq.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jw.hahajie.cn

[C15] 解构 / 展开参数
来源：http://jm.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ei.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://dk.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://im.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gj.yuexingan06.cn

Java: // 无解构
来源：http://br.muxihuayi.cn

Go:   // 无解构
来源：http://xk.huanxung.cn

Ruby: a, b = pair
来源：http://ho.newstarts.cn

C#:   var (a, b) = pair;
来源：http://gz.asd995.cn

[C16] 函数 / 方法重载
来源：http://vp.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gi.colortex.cn

PHP:  // 无重载
来源：http://ew.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://st.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://dk.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wv.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ht.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://mf.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ek.chemitech.net.cn

================================================================================
来源：http://hd.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://uy.gzmigu.cn

================================================================================
来源：http://ss.colortex.cn

[D01] 创建数组 / 列表
来源：http://xo.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ek.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lw.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ih.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dn.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ki.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://sh.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://nx.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ft.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://da.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sn.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qc.colortex.cn

JS:   arr.push(4);
来源：http://zj.szxytkj.cn

TS:   arr.push(4);
来源：http://kg.bookmarksfly.cn

Java: list.add(4);
来源：http://hy.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://wh.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://wz.haigaiapp.cn

C#:   list.Add(4);
来源：http://ip.asd995.cn

[D03] 在指定位置插入元素
来源：http://wu.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://xr.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oi.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ge.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://th.colortex.cn

Java: list.add(0, 0);
来源：http://vq.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sw.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cw.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://ag.nszjky.cn

[D04] 删除元素
来源：http://qp.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nk.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uf.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qn.asd995.cn

TS:   arr.splice(0, 1);
来源：http://qu.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jm.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qj.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yx.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wp.shtwfgs.cn

[D05] 访问与修改元素
来源：http://pm.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gq.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oc.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hy.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://jl.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://em.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://tg.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://md.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yv.shtwfgs.cn

[D06] 数组长度
来源：http://ii.9csxet.cn

Py:   len(arr)
来源：http://pd.wgjwhj.cn

PHP:  count($arr);
来源：http://hm.9csxet.cn

JS:   arr.length
来源：http://wy.jctech888.com.cn

TS:   arr.length
来源：http://pe.newstarts.cn

Java: list.size();
来源：http://fs.hnjuh.cn

Go:   len(arr)
来源：http://qx.huanxung.cn

Ruby: arr.length; arr.size
来源：http://fo.huixiangedu.cn

C#:   list.Count;
来源：http://sf.nicolike.cn

[D07] 切片 / 取子数组
来源：http://zd.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mb.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qq.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://ug.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://tu.nszjky.cn

Java: list.subList(1, 4);
来源：http://ok.colortex.cn

Go:   arr[1:4]
来源：http://bv.521024.cn

Ruby: arr[1, 3]
来源：http://xh.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://gm.yuexingan06.cn

[D08] 合并两个数组
来源：http://js.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://xv.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://mc.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vu.panjiajie.cn

TS:   [...a, ...b];
来源：http://ac.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vj.yuexingan06.cn

Go:   append(a, b...)
来源：http://hp.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://ub.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://yq.wgjwhj.cn

[D09] 排序（升序）
来源：http://nu.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.haigaiapp.cn

PHP:  sort($arr);
来源：http://if.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vb.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qd.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sd.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aq.jianghongdianzi.cn

Ruby: arr.sort
来源：http://np.szsharing.cn

C#:   list.Sort();
来源：http://dp.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ms.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nz.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ns.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zz.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qq.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ce.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sx.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mh.shxzskj.cn

[D11] 反转数组
来源：http://us.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wm.hahajie.cn

PHP:  array_reverse($arr);
来源：http://jg.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wa.nszjky.cn

TS:   [...arr].reverse();
来源：http://ye.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://tu.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://gl.haigaiapp.cn

Ruby: arr.reverse
来源：http://sx.hnjuh.cn

C#:   list.Reverse();
来源：http://tf.bookmarksfly.cn

[D12] 查找元素下标
来源：http://hu.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://hf.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ht.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xp.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tb.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gz.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://jc.lnxyls.cn

Ruby: arr.index(x)
来源：http://xg.nicolike.cn

C#:   list.IndexOf(x);
来源：http://ah.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://rk.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wd.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://db.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://yh.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://cz.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gv.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wq.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sb.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cc.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://mv.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zm.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kb.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://oo.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://gm.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://it.nicolike.cn

Go:   // 手写循环
来源：http://pg.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pq.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lw.szxytkj.cn


<!-- 参考信息 -->