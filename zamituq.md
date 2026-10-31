代发 wailian999

================================================================================
来源：http://uu.chemitech.net.cn

C. 函数与作用域
来源：http://dd.hnjuh.cn

================================================================================
来源：http://vq.yuexingan06.cn

[C01] 定义函数
来源：http://la.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://xd.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oa.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://nq.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rv.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://co.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qc.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://hu.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mf.jctech888.com.cn

[C02] 默认参数
来源：http://lv.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://oh.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://va.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ev.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://di.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cb.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ci.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://pe.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://iy.nszjky.cn

[C03] 可变参数
来源：http://al.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://bc.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xg.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ih.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sn.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cb.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vb.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nm.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bz.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://rw.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fc.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dm.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oq.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ob.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://pm.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://hk.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://rv.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://op.9csxet.cn

[C05] 返回多个值
来源：http://ab.bjjhwx.cn

Py:   return a, b
来源：http://sm.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://uv.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yr.jctech888.com.cn

TS:   return { a, b };
来源：http://nz.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://io.newstarts.cn

Go:   return a, b
来源：http://by.bookmarksfly.cn

Ruby: return a, b
来源：http://sy.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://wx.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://bx.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://wl.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vb.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://pb.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://my.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wg.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ql.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://kc.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fy.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://gq.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nd.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lj.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ou.shxzukj.cn

TS:   arr.map(String)
来源：http://vu.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uv.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://of.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://wc.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ar.colortex.cn

[C08] 闭包
来源：http://vk.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ah.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ma.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xb.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://to.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://di.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dh.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://au.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jq.521024.cn

[C09] 递归
来源：http://me.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sr.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eu.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mc.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gx.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gm.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fm.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dd.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mz.wgjwhj.cn

[C10] 变量作用域
来源：http://ba.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fd.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ba.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tc.nicolike.cn

TS:   同 JS
来源：http://ca.szxytkj.cn

Java: 方法内为块级作用域
来源：http://bi.hnjuh.cn

Go:   花括号块级作用域
来源：http://le.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bu.lnxyls.cn

C#:   块级作用域
来源：http://ul.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ph.shxzukj.cn

Py:   from module import func
来源：http://px.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dp.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tp.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zi.521024.cn

Java: import java.util.List;
来源：http://ol.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jo.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://fk.nicolike.cn

C#:   using System.Text;
来源：http://vl.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://rl.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://ke.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://wk.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://kq.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://aq.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pl.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://oh.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://iw.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lp.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://oa.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pw.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sw.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xt.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qu.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zr.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ov.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eg.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vl.bjjhwx.cn

[C14] 泛型函数
来源：http://er.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mp.nszjky.cn

PHP:  // 无泛型
来源：http://fa.panjiajie.cn

JS:   // 无泛型
来源：http://pg.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kl.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ng.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ds.asd995.cn

Ruby: # 无泛型
来源：http://iz.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vb.szsharing.cn

[C15] 解构 / 展开参数
来源：http://ha.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wh.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://xx.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zt.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cc.nszjky.cn

Java: // 无解构
来源：http://uy.yuexingan06.cn

Go:   // 无解构
来源：http://zg.nszjky.cn

Ruby: a, b = pair
来源：http://dq.9csxet.cn

C#:   var (a, b) = pair;
来源：http://cy.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://hr.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gl.hahajie.cn

PHP:  // 无重载
来源：http://wj.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://av.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://bm.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fg.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://vv.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://nm.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ro.huixinmuqiang.cn

================================================================================
来源：http://rv.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://ca.yuexingan06.cn

================================================================================
来源：http://rh.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://st.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wa.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nm.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://it.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rn.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uh.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://vz.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://hz.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oi.panjiajie.cn

[D02] 追加元素到末尾
来源：http://cg.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uu.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cr.muxihuayi.cn

JS:   arr.push(4);
来源：http://vg.szxytkj.cn

TS:   arr.push(4);
来源：http://gn.bjjhwx.cn

Java: list.add(4);
来源：http://qx.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://cr.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://nt.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://kg.521024.cn

[D03] 在指定位置插入元素
来源：http://pu.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://ox.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wj.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pg.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://bg.shxzukj.cn

Java: list.add(0, 0);
来源：http://sf.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ll.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://md.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://et.shxzukj.cn

[D04] 删除元素
来源：http://us.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yh.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ou.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zj.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://dq.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sr.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hp.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kz.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://on.hahajie.cn

[D05] 访问与修改元素
来源：http://nf.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ko.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wq.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://np.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://ft.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://lr.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://fa.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fv.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lc.521024.cn

[D06] 数组长度
来源：http://uq.lnxyls.cn

Py:   len(arr)
来源：http://dh.wgjwhj.cn

PHP:  count($arr);
来源：http://vw.jctech888.com.cn

JS:   arr.length
来源：http://wt.hnjuh.cn

TS:   arr.length
来源：http://zt.shxzukj.cn

Java: list.size();
来源：http://jw.jianghongdianzi.cn

Go:   len(arr)
来源：http://ac.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://tq.huixiangedu.cn

C#:   list.Count;
来源：http://wj.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://rz.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oo.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jr.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://nf.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://xb.521024.cn

Java: list.subList(1, 4);
来源：http://wi.yuexingan06.cn

Go:   arr[1:4]
来源：http://aj.nicolike.cn

Ruby: arr[1, 3]
来源：http://qo.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://vq.nicolike.cn

[D08] 合并两个数组
来源：http://rq.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://zy.521024.cn

PHP:  array_merge($a, $b);
来源：http://eb.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dt.colortex.cn

TS:   [...a, ...b];
来源：http://mr.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gg.bjjhwx.cn

Go:   append(a, b...)
来源：http://sv.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://yy.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://cj.gzmigu.cn

[D09] 排序（升序）
来源：http://yb.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://do.nicolike.cn

PHP:  sort($arr);
来源：http://el.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ro.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hc.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ox.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://it.yuexingan06.cn

Ruby: arr.sort
来源：http://oy.huixiangedu.cn

C#:   list.Sort();
来源：http://cf.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oq.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gc.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vr.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vq.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ar.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://co.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://or.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zz.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://md.shxzukj.cn

[D11] 反转数组
来源：http://tc.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vj.521024.cn

PHP:  array_reverse($arr);
来源：http://kr.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pu.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://dp.panjiajie.cn

Java: Collections.reverse(list);
来源：http://qm.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://iz.szxytkj.cn

Ruby: arr.reverse
来源：http://pw.9csxet.cn

C#:   list.Reverse();
来源：http://nz.panjiajie.cn

[D12] 查找元素下标
来源：http://yo.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ja.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wy.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ri.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://id.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rs.colortex.cn

Go:   slices.Index(arr, x)
来源：http://bt.nszjky.cn

Ruby: arr.index(x)
来源：http://hm.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://ng.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://yy.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://de.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uv.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://we.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://qg.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rf.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kj.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jq.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://br.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://lo.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zg.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zf.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ot.521024.cn

TS:   arr.map(x => x * 2)
来源：http://jz.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xg.nicolike.cn

Go:   // 手写循环
来源：http://qk.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://og.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mu.szsharing.cn

[D15] 去重
来源：http://bd.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rd.nszjky.cn

PHP:  array_unique($arr);
来源：http://yh.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://ae.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://za.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://va.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://px.gzmigu.cn

Ruby: arr.uniq
来源：http://rx.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://xh.nicolike.cn

[D16] 求和与平均值
来源：http://nv.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kw.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://df.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xh.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ny.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dn.szxytkj.cn

Go:   // 手写循环累加
来源：http://jt.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ky.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://hu.wgjwhj.cn

[D17] 最大值与最小值
来源：http://zs.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://sz.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://co.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fg.szsharing.cn

TS:   Math.max(...arr);
来源：http://ht.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uf.huixiangedu.cn


<!-- 参考信息 -->