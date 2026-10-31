代发 wailian999

Go:   a && b || !c
来源：http://ty.panjiajie.cn

Ruby: a && b || !c
来源：http://ar.yuntaijiaju.cn

C#:   a && b || !c
来源：http://gz.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lt.shtwfgs.cn

Py:   if not data: return
来源：http://nw.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://fx.bjjhwx.cn

JS:   if (!data) return;
来源：http://dh.muxihuayi.cn

TS:   if (!data) return;
来源：http://tp.huixiangedu.cn

Java: if (data == null) return;
来源：http://rs.muxihuayi.cn

Go:   if data == nil { return }
来源：http://sk.haigaiapp.cn

Ruby: return if data.nil?
来源：http://lp.bjjhwx.cn

C#:   if (data == null) return;
来源：http://zk.jianghongdianzi.cn

================================================================================
来源：http://vh.shtwfgs.cn

C. 函数与作用域
来源：http://bp.newstarts.cn

================================================================================
来源：http://po.nicolike.cn

[C01] 定义函数
来源：http://hu.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://on.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tc.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ql.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xm.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dl.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://wp.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sk.newstarts.cn

[C02] 默认参数
来源：http://dv.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://nl.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pa.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://ag.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wm.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ff.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eg.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://dy.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://li.gzmigu.cn

[C03] 可变参数
来源：http://xv.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://cf.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zd.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gj.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://th.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wm.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://il.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://if.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://yj.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mr.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pr.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ui.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oz.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://ze.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://pj.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.521024.cn

C#:   f(a: 1, b: 2)
来源：http://gl.521024.cn

[C05] 返回多个值
来源：http://ad.huixiangedu.cn

Py:   return a, b
来源：http://lz.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://nx.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bn.chemitech.net.cn

TS:   return { a, b };
来源：http://cs.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ga.gzmigu.cn

Go:   return a, b
来源：http://je.nicolike.cn

Ruby: return a, b
来源：http://mo.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://jg.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://ys.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://gw.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lw.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://pu.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://kp.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jp.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xn.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://al.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qm.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ky.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qq.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jo.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gn.panjiajie.cn

TS:   arr.map(String)
来源：http://wz.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zd.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mt.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://tk.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dy.panjiajie.cn

[C08] 闭包
来源：http://ef.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oy.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hi.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pw.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://er.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qq.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wd.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sk.shxzskj.cn

[C09] 递归
来源：http://ox.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zu.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fp.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kf.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lc.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://og.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ts.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pq.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mn.hahajie.cn

[C10] 变量作用域
来源：http://de.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jm.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ss.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ok.shtwfgs.cn

TS:   同 JS
来源：http://mh.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://re.haigaiapp.cn

Go:   花括号块级作用域
来源：http://px.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ej.bookmarksfly.cn

C#:   块级作用域
来源：http://vh.521024.cn

[C11] 模块导入与导出
来源：http://dh.jctech888.com.cn

Py:   from module import func
来源：http://ke.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vt.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sq.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ty.bjjhwx.cn

Java: import java.util.List;
来源：http://jo.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vq.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://vh.chemitech.net.cn

C#:   using System.Text;
来源：http://fr.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://uw.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://nm.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://mo.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://wq.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://yh.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pw.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://vn.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://zt.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://td.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://rd.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ot.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iu.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yp.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dp.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://mu.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bs.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://st.szsharing.cn

[C14] 泛型函数
来源：http://ai.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bl.521024.cn

PHP:  // 无泛型
来源：http://us.newstarts.cn

JS:   // 无泛型
来源：http://gw.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ny.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kg.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ep.chemitech.net.cn

Ruby: # 无泛型
来源：http://md.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oy.nicolike.cn

[C15] 解构 / 展开参数
来源：http://cp.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zc.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://uo.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sb.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://li.wgjwhj.cn

Java: // 无解构
来源：http://rh.panjiajie.cn

Go:   // 无解构
来源：http://pj.panjiajie.cn

Ruby: a, b = pair
来源：http://ct.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://jx.szsharing.cn

[C16] 函数 / 方法重载
来源：http://jz.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://em.huanxung.cn

PHP:  // 无重载
来源：http://xh.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zn.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://oy.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hf.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://bp.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://bv.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.asd995.cn

================================================================================
来源：http://tb.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://rx.huixiangedu.cn

================================================================================
来源：http://cy.asd995.cn

[D01] 创建数组 / 列表
来源：http://ep.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uu.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ue.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ib.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zx.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://th.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://lc.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ud.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sa.shxzskj.cn

[D02] 追加元素到末尾
来源：http://kc.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://si.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://et.wgjwhj.cn

JS:   arr.push(4);
来源：http://hy.shxzukj.cn

TS:   arr.push(4);
来源：http://cj.jianghongdianzi.cn

Java: list.add(4);
来源：http://ao.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://iw.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://nx.shxzukj.cn

C#:   list.Add(4);
来源：http://lx.521024.cn

[D03] 在指定位置插入元素
来源：http://oi.colortex.cn

Py:   arr.insert(0, 0)
来源：http://he.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://za.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kc.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://in.wgjwhj.cn

Java: list.add(0, 0);
来源：http://qx.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bx.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cc.asd995.cn

C#:   list.Insert(0, 0);
来源：http://df.colortex.cn

[D04] 删除元素
来源：http://rg.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ax.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nj.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zs.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://qz.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oj.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kv.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ap.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tk.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://wv.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zd.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xw.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://he.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://zm.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://eb.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://um.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xx.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://or.panjiajie.cn

[D06] 数组长度
来源：http://aa.huixinmuqiang.cn

Py:   len(arr)
来源：http://yv.szxytkj.cn

PHP:  count($arr);
来源：http://rx.szsharing.cn

JS:   arr.length
来源：http://df.yuexingan06.cn

TS:   arr.length
来源：http://ba.shxzskj.cn

Java: list.size();
来源：http://fa.shxzukj.cn

Go:   len(arr)
来源：http://up.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://vl.shtwfgs.cn

C#:   list.Count;
来源：http://mt.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://nj.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yv.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://la.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://rr.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://zv.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ev.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://wb.nicolike.cn

Ruby: arr[1, 3]
来源：http://ie.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://wa.shxzukj.cn

[D08] 合并两个数组
来源：http://vv.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://ck.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://gw.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ei.huixiangedu.cn

TS:   [...a, ...b];
来源：http://nm.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nq.newstarts.cn

Go:   append(a, b...)
来源：http://ug.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://cz.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://xf.9csxet.cn

[D09] 排序（升序）
来源：http://qn.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://be.jctech888.com.cn

PHP:  sort($arr);
来源：http://sc.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ts.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pd.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ca.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bx.asd995.cn

Ruby: arr.sort
来源：http://sr.yuexingan06.cn

C#:   list.Sort();
来源：http://gd.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://my.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bb.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cx.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wu.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cq.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mo.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dj.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sz.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gw.9csxet.cn

[D11] 反转数组
来源：http://dr.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ry.newstarts.cn

PHP:  array_reverse($arr);
来源：http://en.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bh.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://vt.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://ev.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://iq.asd995.cn

Ruby: arr.reverse
来源：http://ry.shtwfgs.cn

C#:   list.Reverse();
来源：http://jw.haigaiapp.cn

[D12] 查找元素下标
来源：http://pf.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://er.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fu.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rn.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://af.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pi.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://yv.hahajie.cn

Ruby: arr.index(x)
来源：http://te.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://yk.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://bj.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ks.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tc.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://bl.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://eg.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bd.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dl.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://te.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dg.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://ja.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://im.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ne.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://vz.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://xl.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jx.lnxyls.cn

Go:   // 手写循环
来源：http://xk.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pk.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gn.chemitech.net.cn

[D15] 去重
来源：http://ny.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wn.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://ja.huanxung.cn

JS:   [...new Set(arr)]
来源：http://pb.huanxung.cn

TS:   [...new Set(arr)]
来源：http://dw.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ec.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wg.521024.cn

Ruby: arr.uniq
来源：http://nl.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://pp.shtwfgs.cn

[D16] 求和与平均值
来源：http://on.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tz.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jb.shxzskj.cn


<!-- 参考信息 -->