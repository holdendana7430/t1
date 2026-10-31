代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kr.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nu.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://et.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bx.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iu.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gg.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://qd.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jl.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qb.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nz.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dq.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://cf.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://cf.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://rt.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://cu.colortex.cn

[C05] 返回多个值
来源：http://dk.9csxet.cn

Py:   return a, b
来源：http://zx.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://yi.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fh.chemitech.net.cn

TS:   return { a, b };
来源：http://ne.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iy.wgjwhj.cn

Go:   return a, b
来源：http://yl.yuntaijiaju.cn

Ruby: return a, b
来源：http://wb.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://of.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ys.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://tt.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pu.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://mc.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://zg.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jc.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sl.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://gf.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ea.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://kr.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mw.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://om.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ei.wgjwhj.cn

TS:   arr.map(String)
来源：http://ub.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dk.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rb.521024.cn

Ruby: arr.map(&:upcase)
来源：http://oi.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vo.newstarts.cn

[C08] 闭包
来源：http://vw.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qg.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nw.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lh.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yk.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tb.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lb.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ul.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nf.chemitech.net.cn

[C09] 递归
来源：http://wh.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jb.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nb.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rn.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pp.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mg.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rm.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vk.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ek.hahajie.cn

[C10] 变量作用域
来源：http://sd.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hr.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ze.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://az.gzmigu.cn

TS:   同 JS
来源：http://oi.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://td.yuexingan06.cn

Go:   花括号块级作用域
来源：http://ry.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qy.haigaiapp.cn

C#:   块级作用域
来源：http://uo.shtwfgs.cn

[C11] 模块导入与导出
来源：http://lv.newstarts.cn

Py:   from module import func
来源：http://ur.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uq.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ek.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tl.hnjuh.cn

Java: import java.util.List;
来源：http://gy.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://my.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://wk.wgjwhj.cn

C#:   using System.Text;
来源：http://gy.521024.cn

[C12] 立即执行函数 IIFE
来源：http://yz.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://bl.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://vp.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://yq.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://vn.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uw.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://oh.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://qt.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wi.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://iy.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://su.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tk.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lq.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fq.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://mj.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zj.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ue.huixiangedu.cn

[C14] 泛型函数
来源：http://bm.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ay.newstarts.cn

PHP:  // 无泛型
来源：http://gg.haigaiapp.cn

JS:   // 无泛型
来源：http://mq.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ua.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uz.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ip.gzmigu.cn

Ruby: # 无泛型
来源：http://ng.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sk.huanxung.cn

[C15] 解构 / 展开参数
来源：http://zg.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ca.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ka.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tz.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fy.muxihuayi.cn

Java: // 无解构
来源：http://ds.huanxung.cn

Go:   // 无解构
来源：http://br.yuexingan06.cn

Ruby: a, b = pair
来源：http://so.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://sc.colortex.cn

[C16] 函数 / 方法重载
来源：http://gj.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://no.huixiangedu.cn

PHP:  // 无重载
来源：http://nq.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rq.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tm.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://de.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://nh.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://bv.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kb.lnxyls.cn

================================================================================
来源：http://wc.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://vx.szxytkj.cn

================================================================================
来源：http://ib.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://yx.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ck.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dl.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ob.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fs.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tg.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rc.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://nr.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yh.szxytkj.cn

[D02] 追加元素到末尾
来源：http://qo.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sd.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tc.hahajie.cn

JS:   arr.push(4);
来源：http://cy.chemitech.net.cn

TS:   arr.push(4);
来源：http://hw.9csxet.cn

Java: list.add(4);
来源：http://qa.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://zl.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://hd.asd995.cn

C#:   list.Add(4);
来源：http://nq.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://mp.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://tz.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zk.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cp.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://hq.huanxung.cn

Java: list.add(0, 0);
来源：http://aw.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ux.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xt.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://bo.9csxet.cn

[D04] 删除元素
来源：http://vl.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ki.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cc.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sx.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://fg.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ca.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cn.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pp.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sf.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://ye.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yo.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rn.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jg.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://wh.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ne.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ed.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wf.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ns.muxihuayi.cn

[D06] 数组长度
来源：http://zz.521024.cn

Py:   len(arr)
来源：http://ki.chemitech.net.cn

PHP:  count($arr);
来源：http://wy.9csxet.cn

JS:   arr.length
来源：http://bv.hnjuh.cn

TS:   arr.length
来源：http://sr.szxytkj.cn

Java: list.size();
来源：http://wx.szsharing.cn

Go:   len(arr)
来源：http://es.szsharing.cn

Ruby: arr.length; arr.size
来源：http://dt.huixinmuqiang.cn

C#:   list.Count;
来源：http://zc.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://wb.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fr.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xm.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ao.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ht.nicolike.cn

Java: list.subList(1, 4);
来源：http://vl.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ah.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://bp.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://wr.hahajie.cn

[D08] 合并两个数组
来源：http://va.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://tu.colortex.cn

PHP:  array_merge($a, $b);
来源：http://zc.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cx.newstarts.cn

TS:   [...a, ...b];
来源：http://fs.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bk.newstarts.cn

Go:   append(a, b...)
来源：http://ug.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://ho.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://uo.9csxet.cn

[D09] 排序（升序）
来源：http://vb.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://cl.hnjuh.cn

PHP:  sort($arr);
来源：http://as.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ge.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cg.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ry.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wr.521024.cn

Ruby: arr.sort
来源：http://fe.szxytkj.cn

C#:   list.Sort();
来源：http://ly.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lg.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ub.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nc.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pu.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ku.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ts.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ll.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kh.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tb.gzmigu.cn

[D11] 反转数组
来源：http://mr.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ep.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://ys.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hh.hahajie.cn

TS:   [...arr].reverse();
来源：http://hz.lnxyls.cn

Java: Collections.reverse(list);
来源：http://ec.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://lg.asd995.cn

Ruby: arr.reverse
来源：http://wd.hnjuh.cn

C#:   list.Reverse();
来源：http://xy.shxzskj.cn

[D12] 查找元素下标
来源：http://sc.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://fa.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://he.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lf.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mw.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://iv.szxytkj.cn

Ruby: arr.index(x)
来源：http://ef.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ig.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://wd.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dq.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fq.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://lp.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ji.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ge.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nr.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://di.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pm.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://un.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vg.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ua.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://yg.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://sw.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vh.bookmarksfly.cn

Go:   // 手写循环
来源：http://ad.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sx.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wt.panjiajie.cn

[D15] 去重
来源：http://nk.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sk.szxytkj.cn

PHP:  array_unique($arr);
来源：http://xl.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://sy.huanxung.cn

TS:   [...new Set(arr)]
来源：http://rs.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://op.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wj.bjjhwx.cn

Ruby: arr.uniq
来源：http://vg.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://jh.szsharing.cn

[D16] 求和与平均值
来源：http://qj.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ri.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tn.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ja.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zz.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ii.muxihuayi.cn

Go:   // 手写循环累加
来源：http://jf.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://af.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://jy.muxihuayi.cn

[D17] 最大值与最小值
来源：http://je.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://zr.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://qh.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mb.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://jm.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cu.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wx.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://nq.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://jz.asd995.cn

[D18] 扁平化嵌套数组
来源：http://xw.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lv.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://hk.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gs.wgjwhj.cn

TS:   nested.flat();
来源：http://pe.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xd.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://hf.jctech888.com.cn

Ruby: nested.flatten
来源：http://tj.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://av.chemitech.net.cn

[D19] 按字段分组
来源：http://io.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gv.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://la.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ow.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rs.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tu.521024.cn

Go:   // 手写 map[string][]T
来源：http://fx.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lt.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pj.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://zd.bjjhwx.cn

Py:   Counter(arr)
来源：http://pz.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://yd.colortex.cn


<!-- 参考信息 -->