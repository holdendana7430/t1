代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uz.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ad.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ls.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cl.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ui.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tu.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://vw.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rx.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xx.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ty.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ii.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://uq.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://wo.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ru.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://nt.huixinmuqiang.cn

[C05] 返回多个值
来源：http://em.newstarts.cn

Py:   return a, b
来源：http://ox.huanxung.cn

PHP:  return [$a, $b];
来源：http://od.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rm.bjjhwx.cn

TS:   return { a, b };
来源：http://vd.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tz.wgjwhj.cn

Go:   return a, b
来源：http://gh.haigaiapp.cn

Ruby: return a, b
来源：http://vk.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://wa.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://sm.521024.cn

Py:   square = lambda x: x * x
来源：http://mz.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bo.gzmigu.cn

JS:   const square = x => x * x;
来源：http://kq.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://jm.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kv.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ot.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://km.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qd.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://qn.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cb.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uv.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yg.huixiangedu.cn

TS:   arr.map(String)
来源：http://cq.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uv.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ke.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://sn.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ro.haigaiapp.cn

[C08] 闭包
来源：http://ds.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wb.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xw.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zc.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fi.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wr.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ib.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kb.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tu.yuntaijiaju.cn

[C09] 递归
来源：http://he.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ig.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bi.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ob.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://az.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cf.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tl.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vm.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ug.nszjky.cn

[C10] 变量作用域
来源：http://qw.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tu.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fn.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://id.lnxyls.cn

TS:   同 JS
来源：http://qm.szsharing.cn

Java: 方法内为块级作用域
来源：http://xs.hahajie.cn

Go:   花括号块级作用域
来源：http://pi.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tc.muxihuayi.cn

C#:   块级作用域
来源：http://sa.wgjwhj.cn

[C11] 模块导入与导出
来源：http://xt.nicolike.cn

Py:   from module import func
来源：http://vo.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fy.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xf.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ty.wgjwhj.cn

Java: import java.util.List;
来源：http://mt.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lz.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://zy.bookmarksfly.cn

C#:   using System.Text;
来源：http://rg.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://pc.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://hq.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://wh.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://hs.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://bx.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ph.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://tn.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://qc.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://et.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://au.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jy.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fe.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yz.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jn.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pq.521024.cn

Go:   func add(a, b int) int
来源：http://xq.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yh.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://co.bookmarksfly.cn

[C14] 泛型函数
来源：http://yb.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bb.bjjhwx.cn

PHP:  // 无泛型
来源：http://sv.asd995.cn

JS:   // 无泛型
来源：http://rf.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ja.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xt.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jw.nszjky.cn

Ruby: # 无泛型
来源：http://oy.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ow.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://rk.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zy.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ar.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yw.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pb.muxihuayi.cn

Java: // 无解构
来源：http://fv.521024.cn

Go:   // 无解构
来源：http://op.9csxet.cn

Ruby: a, b = pair
来源：http://ig.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://ne.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://le.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://et.szxytkj.cn

PHP:  // 无重载
来源：http://lh.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tv.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://jc.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ch.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://hc.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://no.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hs.szxytkj.cn

================================================================================
来源：http://pi.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://at.haigaiapp.cn

================================================================================
来源：http://pr.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://lp.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://th.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://at.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sa.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jx.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ub.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ns.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://kg.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qz.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://km.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fk.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fo.nszjky.cn

JS:   arr.push(4);
来源：http://vb.gzmigu.cn

TS:   arr.push(4);
来源：http://hz.huixinmuqiang.cn

Java: list.add(4);
来源：http://ea.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://si.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://fz.hahajie.cn

C#:   list.Add(4);
来源：http://nq.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://eg.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://wu.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sg.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vr.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://qz.bjjhwx.cn

Java: list.add(0, 0);
来源：http://xb.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vk.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zb.521024.cn

C#:   list.Insert(0, 0);
来源：http://eq.bookmarksfly.cn

[D04] 删除元素
来源：http://of.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yr.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xt.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xo.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://vv.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mg.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ud.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wi.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uv.shxzukj.cn

[D05] 访问与修改元素
来源：http://kv.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jx.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ki.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ib.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://md.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://px.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://tu.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xx.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uz.yuntaijiaju.cn

[D06] 数组长度
来源：http://kz.jianghongdianzi.cn

Py:   len(arr)
来源：http://cl.panjiajie.cn

PHP:  count($arr);
来源：http://sz.chemitech.net.cn

JS:   arr.length
来源：http://cr.nicolike.cn

TS:   arr.length
来源：http://bk.9csxet.cn

Java: list.size();
来源：http://us.szsharing.cn

Go:   len(arr)
来源：http://hc.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://un.colortex.cn

C#:   list.Count;
来源：http://dq.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://hm.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eu.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ek.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ej.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://rn.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://ja.jctech888.com.cn

Go:   arr[1:4]
来源：http://ty.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vv.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://hx.9csxet.cn

[D08] 合并两个数组
来源：http://zv.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://uj.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://ow.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qf.nicolike.cn

TS:   [...a, ...b];
来源：http://um.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ir.chemitech.net.cn

Go:   append(a, b...)
来源：http://ye.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://bh.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://ya.huixiangedu.cn

[D09] 排序（升序）
来源：http://jb.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://un.shtwfgs.cn

PHP:  sort($arr);
来源：http://zt.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sa.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tc.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wm.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mb.hnjuh.cn

Ruby: arr.sort
来源：http://wy.nszjky.cn

C#:   list.Sort();
来源：http://sr.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mw.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://st.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ny.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://to.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oq.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tt.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://us.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://li.haigaiapp.cn

[D11] 反转数组
来源：http://tw.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fp.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://lm.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oy.shxzskj.cn

TS:   [...arr].reverse();
来源：http://rz.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://mf.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://kw.521024.cn

Ruby: arr.reverse
来源：http://my.wgjwhj.cn

C#:   list.Reverse();
来源：http://oc.newstarts.cn

[D12] 查找元素下标
来源：http://bq.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://go.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://je.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pn.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yy.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://td.shxzskj.cn

Ruby: arr.index(x)
来源：http://aq.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ro.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://uw.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vf.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jo.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://lt.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://jy.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gq.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qx.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iz.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://zc.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pk.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ki.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://et.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://sy.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wu.shxzukj.cn

Go:   // 手写循环
来源：http://wn.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://up.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wm.colortex.cn

[D15] 去重
来源：http://bu.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ph.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://dc.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://fo.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://rp.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://st.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hk.haigaiapp.cn

Ruby: arr.uniq
来源：http://vo.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://sh.wgjwhj.cn

[D16] 求和与平均值
来源：http://lv.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dk.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zd.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ox.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zy.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mr.bjjhwx.cn

Go:   // 手写循环累加
来源：http://rv.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://os.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://tq.szsharing.cn

[D17] 最大值与最小值
来源：http://lf.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ip.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://jm.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gz.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://or.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zp.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://at.colortex.cn

Ruby: arr.max;  arr.min
来源：http://xs.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://tt.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://ve.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ep.521024.cn

PHP:  array_merge(...$nested);
来源：http://wk.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wb.shxzskj.cn

TS:   nested.flat();
来源：http://dd.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lb.9csxet.cn

Go:   // 手写双层循环
来源：http://fv.hahajie.cn

Ruby: nested.flatten
来源：http://om.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jg.huixinmuqiang.cn

[D19] 按字段分组
来源：http://vz.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ch.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dm.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dn.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zp.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ep.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://gk.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mf.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jk.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://hk.9csxet.cn

Py:   Counter(arr)
来源：http://kg.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://rx.bookmarksfly.cn


<!-- 参考信息 -->