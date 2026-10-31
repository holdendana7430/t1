代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hi.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pa.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://px.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yj.huixiangedu.cn

[C02] 默认参数
来源：http://ho.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://du.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nz.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://jk.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ma.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zx.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aa.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://bl.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://cu.haigaiapp.cn

[C03] 可变参数
来源：http://ij.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://tg.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ku.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dw.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ur.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pt.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cc.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rw.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cl.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://pn.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cb.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lt.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vm.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bk.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://co.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://hx.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://wq.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://fd.yuexingan06.cn

[C05] 返回多个值
来源：http://wa.jianghongdianzi.cn

Py:   return a, b
来源：http://yw.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://gm.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wi.jianghongdianzi.cn

TS:   return { a, b };
来源：http://hg.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tz.colortex.cn

Go:   return a, b
来源：http://hq.nszjky.cn

Ruby: return a, b
来源：http://uh.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://me.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://jo.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://wb.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://na.shxzskj.cn

JS:   const square = x => x * x;
来源：http://ut.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://go.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://si.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://en.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://pk.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ut.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://zz.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xv.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pj.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tb.bookmarksfly.cn

TS:   arr.map(String)
来源：http://fz.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ni.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ii.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://mu.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ne.wgjwhj.cn

[C08] 闭包
来源：http://kl.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xo.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bt.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ue.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sk.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wb.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zv.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rg.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pk.colortex.cn

[C09] 递归
来源：http://oe.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qg.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ns.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uz.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wc.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://il.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ve.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ly.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ga.521024.cn

[C10] 变量作用域
来源：http://pv.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fn.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zk.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ts.szsharing.cn

TS:   同 JS
来源：http://zo.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ya.hnjuh.cn

Go:   花括号块级作用域
来源：http://ao.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kv.wgjwhj.cn

C#:   块级作用域
来源：http://pt.haigaiapp.cn

[C11] 模块导入与导出
来源：http://qx.huixiangedu.cn

Py:   from module import func
来源：http://vp.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bu.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ae.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bd.huanxung.cn

Java: import java.util.List;
来源：http://zt.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hd.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ub.bjjhwx.cn

C#:   using System.Text;
来源：http://nx.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://io.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://xr.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://dm.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://mk.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://vk.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nh.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://id.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://pk.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vb.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://cl.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://js.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://og.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yg.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xu.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://mp.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xd.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://et.yuntaijiaju.cn

[C14] 泛型函数
来源：http://yl.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ey.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ba.9csxet.cn

JS:   // 无泛型
来源：http://cy.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qb.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wq.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dm.hnjuh.cn

Ruby: # 无泛型
来源：http://uk.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sc.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://mx.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oc.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://qm.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zs.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wp.jctech888.com.cn

Java: // 无解构
来源：http://am.9csxet.cn

Go:   // 无解构
来源：http://gm.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://yc.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://xf.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://qe.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rg.hnjuh.cn

PHP:  // 无重载
来源：http://jh.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://em.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://tp.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hd.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://no.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://uc.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gw.jctech888.com.cn

================================================================================
来源：http://ca.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://hn.bjjhwx.cn

================================================================================
来源：http://le.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://vy.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fc.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mc.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yl.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ce.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nn.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://sf.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://ja.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bt.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://zt.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yz.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nm.huanxung.cn

JS:   arr.push(4);
来源：http://ej.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://gm.wgjwhj.cn

Java: list.add(4);
来源：http://wb.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://gm.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.gzmigu.cn

C#:   list.Add(4);
来源：http://ta.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://gv.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://av.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qr.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://av.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://bi.chemitech.net.cn

Java: list.add(0, 0);
来源：http://dc.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fq.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kc.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://ix.shxzukj.cn

[D04] 删除元素
来源：http://eo.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fo.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kh.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qo.521024.cn

TS:   arr.splice(0, 1);
来源：http://uo.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sv.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gz.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gs.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xs.muxihuayi.cn

[D05] 访问与修改元素
来源：http://gl.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vt.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lz.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dd.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://dv.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://pl.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://xh.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nw.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bp.colortex.cn

[D06] 数组长度
来源：http://rb.asd995.cn

Py:   len(arr)
来源：http://oj.asd995.cn

PHP:  count($arr);
来源：http://vv.szxytkj.cn

JS:   arr.length
来源：http://yl.521024.cn

TS:   arr.length
来源：http://rc.bjjhwx.cn

Java: list.size();
来源：http://jx.haigaiapp.cn

Go:   len(arr)
来源：http://oj.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://zk.shtwfgs.cn

C#:   list.Count;
来源：http://ld.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://oc.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ho.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nb.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://wf.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://dj.521024.cn

Java: list.subList(1, 4);
来源：http://up.hnjuh.cn

Go:   arr[1:4]
来源：http://cg.asd995.cn

Ruby: arr[1, 3]
来源：http://oq.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://jj.muxihuayi.cn

[D08] 合并两个数组
来源：http://pp.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://ve.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://wf.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ad.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://rc.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vg.muxihuayi.cn

Go:   append(a, b...)
来源：http://xp.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://om.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://qp.chemitech.net.cn

[D09] 排序（升序）
来源：http://sb.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://pr.newstarts.cn

PHP:  sort($arr);
来源：http://kt.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lz.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hi.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ex.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ao.521024.cn

Ruby: arr.sort
来源：http://wg.yuexingan06.cn

C#:   list.Sort();
来源：http://zz.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gg.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://my.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sh.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oo.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ll.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qt.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bq.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uw.muxihuayi.cn

[D11] 反转数组
来源：http://bs.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xe.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://dl.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rw.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://pd.9csxet.cn

Java: Collections.reverse(list);
来源：http://nv.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://ev.colortex.cn

Ruby: arr.reverse
来源：http://cb.bookmarksfly.cn

C#:   list.Reverse();
来源：http://wf.gzmigu.cn

[D12] 查找元素下标
来源：http://hz.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://xt.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://va.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xs.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dm.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fb.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://vp.huanxung.cn

Ruby: arr.index(x)
来源：http://wc.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://ih.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://wu.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qq.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rq.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://yf.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://rr.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xw.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://so.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mx.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jj.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://tt.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wb.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gi.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://eb.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://py.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ch.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ky.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://er.yuexingan06.cn

[D15] 去重
来源：http://ba.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eh.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://pw.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://yo.521024.cn

TS:   [...new Set(arr)]
来源：http://xn.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rp.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xu.haigaiapp.cn

Ruby: arr.uniq
来源：http://mp.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://kq.asd995.cn

[D16] 求和与平均值
来源：http://sn.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vs.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pc.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ps.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://or.huixiangedu.cn

Go:   // 手写循环累加
来源：http://sx.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qb.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ph.szsharing.cn

[D17] 最大值与最小值
来源：http://jx.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://xb.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ru.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yw.asd995.cn

TS:   Math.max(...arr);
来源：http://rq.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rm.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ab.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://yf.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://tk.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://xz.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zu.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://pa.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ud.asd995.cn

TS:   nested.flat();
来源：http://df.nszjky.cn


<!-- 参考信息 -->