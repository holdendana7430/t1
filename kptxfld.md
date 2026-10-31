代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://eq.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ks.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yt.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://cu.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://zb.huixinmuqiang.cn

[C03] 可变参数
来源：http://kd.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://ni.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lm.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yo.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ih.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cd.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gq.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oo.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://yp.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qt.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ea.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vt.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xo.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://rp.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://yx.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ro.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://mn.shxzukj.cn

[C05] 返回多个值
来源：http://bk.wgjwhj.cn

Py:   return a, b
来源：http://uu.panjiajie.cn

PHP:  return [$a, $b];
来源：http://xy.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xv.lnxyls.cn

TS:   return { a, b };
来源：http://tj.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oq.colortex.cn

Go:   return a, b
来源：http://nj.huixinmuqiang.cn

Ruby: return a, b
来源：http://pb.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://is.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://xz.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://mf.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iy.newstarts.cn

JS:   const square = x => x * x;
来源：http://wp.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://uo.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pf.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://js.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ec.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lx.521024.cn

[C07] 把函数作为参数传入
来源：http://dn.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ki.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sf.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ms.nicolike.cn

TS:   arr.map(String)
来源：http://hi.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ni.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ud.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://se.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yo.jctech888.com.cn

[C08] 闭包
来源：http://um.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wo.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rx.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wn.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wm.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wr.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ik.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oa.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qc.521024.cn

[C09] 递归
来源：http://yq.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xj.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tm.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://up.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ml.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kd.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cj.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://id.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xs.panjiajie.cn

[C10] 变量作用域
来源：http://am.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vb.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ig.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rn.newstarts.cn

TS:   同 JS
来源：http://va.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://mj.szsharing.cn

Go:   花括号块级作用域
来源：http://by.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ic.jianghongdianzi.cn

C#:   块级作用域
来源：http://sw.muxihuayi.cn

[C11] 模块导入与导出
来源：http://sg.hnjuh.cn

Py:   from module import func
来源：http://uj.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://io.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cd.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pk.shtwfgs.cn

Java: import java.util.List;
来源：http://oj.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ik.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://fp.521024.cn

C#:   using System.Text;
来源：http://sw.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://cv.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://ve.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://qh.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://bv.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://do.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pl.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://il.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://mu.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mu.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://jw.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kv.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xf.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tx.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://id.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://cy.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hi.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cg.haigaiapp.cn

[C14] 泛型函数
来源：http://uk.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tl.yuexingan06.cn

PHP:  // 无泛型
来源：http://ue.panjiajie.cn

JS:   // 无泛型
来源：http://lu.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bb.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://be.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kd.muxihuayi.cn

Ruby: # 无泛型
来源：http://wn.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://im.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://tc.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zf.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://rb.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bt.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nt.9csxet.cn

Java: // 无解构
来源：http://vi.nszjky.cn

Go:   // 无解构
来源：http://bb.hnjuh.cn

Ruby: a, b = pair
来源：http://ap.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://dy.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://rm.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tc.jctech888.com.cn

PHP:  // 无重载
来源：http://rr.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xq.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://il.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ju.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://ta.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://an.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sk.szxytkj.cn

================================================================================
来源：http://ep.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://wn.panjiajie.cn

================================================================================
来源：http://mh.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://ks.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://db.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ux.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bf.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fs.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://op.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://jr.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://px.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xb.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://hn.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jg.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://to.521024.cn

JS:   arr.push(4);
来源：http://ga.szxytkj.cn

TS:   arr.push(4);
来源：http://tc.huixiangedu.cn

Java: list.add(4);
来源：http://is.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://lk.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://uu.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://wl.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://xf.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://bm.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://em.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cc.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://em.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://cc.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vo.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tx.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://st.huanxung.cn

[D04] 删除元素
来源：http://ev.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bs.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://de.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hv.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ft.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zi.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kj.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yz.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wg.shxzukj.cn

[D05] 访问与修改元素
来源：http://rz.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ok.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rn.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tc.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://na.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://ac.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://yo.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pk.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jk.muxihuayi.cn

[D06] 数组长度
来源：http://rm.yuntaijiaju.cn

Py:   len(arr)
来源：http://vr.bjjhwx.cn

PHP:  count($arr);
来源：http://fb.bjjhwx.cn

JS:   arr.length
来源：http://oh.shxzukj.cn

TS:   arr.length
来源：http://oc.asd995.cn

Java: list.size();
来源：http://qt.panjiajie.cn

Go:   len(arr)
来源：http://ma.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://dk.shxzukj.cn

C#:   list.Count;
来源：http://iu.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://nw.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hs.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bl.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://mk.521024.cn

TS:   arr.slice(1, 4);
来源：http://by.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://xt.hahajie.cn

Go:   arr[1:4]
来源：http://wn.9csxet.cn

Ruby: arr[1, 3]
来源：http://th.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://pu.colortex.cn

[D08] 合并两个数组
来源：http://oo.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ij.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://nl.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vh.newstarts.cn

TS:   [...a, ...b];
来源：http://xc.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://he.yuexingan06.cn

Go:   append(a, b...)
来源：http://lh.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://pb.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://ai.bjjhwx.cn

[D09] 排序（升序）
来源：http://xm.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.jctech888.com.cn

PHP:  sort($arr);
来源：http://cs.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jt.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jb.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qp.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://db.szsharing.cn

Ruby: arr.sort
来源：http://na.hahajie.cn

C#:   list.Sort();
来源：http://ap.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mp.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qf.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kr.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ir.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xq.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mq.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oi.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qo.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ik.521024.cn

[D11] 反转数组
来源：http://mw.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pe.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://go.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sh.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ys.lnxyls.cn

Java: Collections.reverse(list);
来源：http://in.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://rm.nszjky.cn

Ruby: arr.reverse
来源：http://fk.gzmigu.cn

C#:   list.Reverse();
来源：http://qw.muxihuayi.cn

[D12] 查找元素下标
来源：http://vm.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://fc.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://od.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ut.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bn.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lx.521024.cn

Go:   slices.Index(arr, x)
来源：http://db.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://vm.9csxet.cn

C#:   list.IndexOf(x);
来源：http://ca.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://eu.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yv.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dj.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://ty.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ev.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cl.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gt.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oy.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bk.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://wu.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uc.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://bl.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://cu.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vk.colortex.cn

Go:   // 手写循环
来源：http://bj.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zd.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rn.bookmarksfly.cn

[D15] 去重
来源：http://sy.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ye.shxzskj.cn

PHP:  array_unique($arr);
来源：http://tw.huanxung.cn

JS:   [...new Set(arr)]
来源：http://ni.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://bx.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oa.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xv.yuexingan06.cn

Ruby: arr.uniq
来源：http://xp.colortex.cn

C#:   list.Distinct().ToList()
来源：http://vk.gzmigu.cn

[D16] 求和与平均值
来源：http://vi.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qe.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://we.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rd.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ao.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qb.asd995.cn

Go:   // 手写循环累加
来源：http://mt.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dn.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://xr.hahajie.cn

[D17] 最大值与最小值
来源：http://qt.colortex.cn

Py:   max(arr);  min(arr)
来源：http://wp.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://cj.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vw.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://pe.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rf.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mu.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://fi.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://ww.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://py.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zk.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://yx.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wi.huanxung.cn

TS:   nested.flat();
来源：http://id.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cf.jctech888.com.cn

Go:   // 手写双层循环
来源：http://jj.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://pj.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://en.wgjwhj.cn

[D19] 按字段分组
来源：http://va.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tm.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hc.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pt.newstarts.cn


<!-- 参考信息 -->