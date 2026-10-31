代发 wailian999

Py:   if not data: return
来源：http://me.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://eq.haigaiapp.cn

JS:   if (!data) return;
来源：http://gb.szsharing.cn

TS:   if (!data) return;
来源：http://qm.jctech888.com.cn

Java: if (data == null) return;
来源：http://bk.panjiajie.cn

Go:   if data == nil { return }
来源：http://wx.jctech888.com.cn

Ruby: return if data.nil?
来源：http://dg.asd995.cn

C#:   if (data == null) return;
来源：http://ki.shtwfgs.cn

================================================================================
来源：http://jz.huixinmuqiang.cn

C. 函数与作用域
来源：http://ll.nicolike.cn

================================================================================
来源：http://ln.nszjky.cn

[C01] 定义函数
来源：http://ws.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://cx.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://gs.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rr.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rx.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vu.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://kn.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kr.panjiajie.cn

[C02] 默认参数
来源：http://es.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://he.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qq.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://bo.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tj.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xq.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ik.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ud.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ok.shtwfgs.cn

[C03] 可变参数
来源：http://hn.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://sm.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ui.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ak.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pb.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://km.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rt.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xz.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tp.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://kh.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wt.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ka.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rg.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pu.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://be.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ie.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://hu.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://xd.jctech888.com.cn

[C05] 返回多个值
来源：http://lc.szxytkj.cn

Py:   return a, b
来源：http://ac.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://sx.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bf.jianghongdianzi.cn

TS:   return { a, b };
来源：http://rc.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dr.521024.cn

Go:   return a, b
来源：http://iu.hahajie.cn

Ruby: return a, b
来源：http://vs.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://bm.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://up.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://yv.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kv.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://nx.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://es.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oz.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://if.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://qs.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bl.newstarts.cn

[C07] 把函数作为参数传入
来源：http://xc.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wt.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://by.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pe.shtwfgs.cn

TS:   arr.map(String)
来源：http://sz.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wm.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tp.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://kq.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lo.521024.cn

[C08] 闭包
来源：http://qq.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ev.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ab.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qt.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dt.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bu.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://td.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://we.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gb.asd995.cn

[C09] 递归
来源：http://ie.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kr.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fh.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oh.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gs.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yb.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://de.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ue.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ep.hahajie.cn

[C10] 变量作用域
来源：http://er.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://js.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oc.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qm.lnxyls.cn

TS:   同 JS
来源：http://yx.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://vk.hnjuh.cn

Go:   花括号块级作用域
来源：http://dr.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gp.gzmigu.cn

C#:   块级作用域
来源：http://qt.szxytkj.cn

[C11] 模块导入与导出
来源：http://sa.nicolike.cn

Py:   from module import func
来源：http://lx.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mb.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mh.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gk.szxytkj.cn

Java: import java.util.List;
来源：http://um.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sj.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://wl.colortex.cn

C#:   using System.Text;
来源：http://in.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://mb.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://lp.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://sm.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://wo.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://or.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ys.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ab.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://ep.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kr.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://cx.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lk.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zw.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xz.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://as.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dg.shxzukj.cn

Go:   func add(a, b int) int
来源：http://xe.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sk.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gt.jctech888.com.cn

[C14] 泛型函数
来源：http://oh.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wg.newstarts.cn

PHP:  // 无泛型
来源：http://hd.yuntaijiaju.cn

JS:   // 无泛型
来源：http://fv.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uw.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ic.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://th.muxihuayi.cn

Ruby: # 无泛型
来源：http://gm.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qq.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://ab.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xr.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ah.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xb.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xu.bookmarksfly.cn

Java: // 无解构
来源：http://qc.hnjuh.cn

Go:   // 无解构
来源：http://pe.asd995.cn

Ruby: a, b = pair
来源：http://bd.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://id.hahajie.cn

[C16] 函数 / 方法重载
来源：http://tk.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zt.hnjuh.cn

PHP:  // 无重载
来源：http://zz.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jw.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://fv.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yd.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ll.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://oq.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://og.yuntaijiaju.cn

================================================================================
来源：http://kx.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://yv.asd995.cn

================================================================================
来源：http://hm.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://pj.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rt.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://es.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qo.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pq.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hm.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ku.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://bk.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nj.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://ec.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://he.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bk.521024.cn

JS:   arr.push(4);
来源：http://uw.hahajie.cn

TS:   arr.push(4);
来源：http://hc.jianghongdianzi.cn

Java: list.add(4);
来源：http://vb.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://mo.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://lc.shtwfgs.cn

C#:   list.Add(4);
来源：http://xf.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://ma.asd995.cn

Py:   arr.insert(0, 0)
来源：http://fh.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bw.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mw.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://pd.9csxet.cn

Java: list.add(0, 0);
来源：http://oz.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xj.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ar.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://uy.521024.cn

[D04] 删除元素
来源：http://vo.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uv.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ld.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jh.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://pc.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yp.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xj.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dc.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hx.shxzukj.cn

[D05] 访问与修改元素
来源：http://nn.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://do.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sw.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ut.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://zz.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://wt.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://zu.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vm.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kr.nszjky.cn

[D06] 数组长度
来源：http://bc.lnxyls.cn

Py:   len(arr)
来源：http://hy.yuexingan06.cn

PHP:  count($arr);
来源：http://vt.gzmigu.cn

JS:   arr.length
来源：http://hz.bookmarksfly.cn

TS:   arr.length
来源：http://gy.muxihuayi.cn

Java: list.size();
来源：http://ds.colortex.cn

Go:   len(arr)
来源：http://bu.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://ll.shxzskj.cn

C#:   list.Count;
来源：http://kr.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://ym.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wc.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kz.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://wy.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://xp.asd995.cn

Java: list.subList(1, 4);
来源：http://dt.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://qd.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ih.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://eu.huanxung.cn

[D08] 合并两个数组
来源：http://cp.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://qv.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://cs.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pz.panjiajie.cn

TS:   [...a, ...b];
来源：http://fq.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yq.9csxet.cn

Go:   append(a, b...)
来源：http://yh.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://hg.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://zo.hnjuh.cn

[D09] 排序（升序）
来源：http://mh.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ev.newstarts.cn

PHP:  sort($arr);
来源：http://qn.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cg.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pn.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cm.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hg.huixiangedu.cn

Ruby: arr.sort
来源：http://ah.bjjhwx.cn

C#:   list.Sort();
来源：http://as.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hd.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uz.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rt.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pn.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tp.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fw.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ks.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bf.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yw.shxzskj.cn

[D11] 反转数组
来源：http://nz.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qv.newstarts.cn

PHP:  array_reverse($arr);
来源：http://dn.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lk.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://bx.nicolike.cn

Java: Collections.reverse(list);
来源：http://sb.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://sl.shtwfgs.cn

Ruby: arr.reverse
来源：http://mn.szxytkj.cn

C#:   list.Reverse();
来源：http://ns.newstarts.cn

[D12] 查找元素下标
来源：http://fl.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://sf.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iz.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bl.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sa.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aa.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://qc.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://cd.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://fm.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://jg.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uc.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uf.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://jt.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://ot.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ln.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vq.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gv.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pw.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://sy.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ff.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ly.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://hz.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://kz.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eg.asd995.cn

Go:   // 手写循环
来源：http://lk.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yb.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qg.lnxyls.cn

[D15] 去重
来源：http://cf.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zv.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ce.asd995.cn

JS:   [...new Set(arr)]
来源：http://er.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://pc.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nl.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ie.szsharing.cn

Ruby: arr.uniq
来源：http://ty.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://lt.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://pc.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sd.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lo.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wv.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ey.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yr.521024.cn

Go:   // 手写循环累加
来源：http://ym.jctech888.com.cn


<!-- 参考信息 -->