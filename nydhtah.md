代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://ci.chemitech.net.cn

[C03] 可变参数
来源：http://sw.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://yh.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jd.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rv.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ac.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jh.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dm.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pl.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://po.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://tq.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cr.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gj.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://og.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gv.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://mi.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://yp.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://gf.521024.cn

C#:   f(a: 1, b: 2)
来源：http://cz.haigaiapp.cn

[C05] 返回多个值
来源：http://ld.bookmarksfly.cn

Py:   return a, b
来源：http://so.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://gl.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xd.haigaiapp.cn

TS:   return { a, b };
来源：http://ri.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sq.panjiajie.cn

Go:   return a, b
来源：http://qs.jctech888.com.cn

Ruby: return a, b
来源：http://gl.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://fx.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://ji.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://sh.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nx.szsharing.cn

JS:   const square = x => x * x;
来源：http://vw.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://on.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://en.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pn.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://xi.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vb.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://be.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mr.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qc.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yh.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://ih.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uc.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zp.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://mz.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xt.szxytkj.cn

[C08] 闭包
来源：http://rr.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kg.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dc.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pa.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hk.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nu.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mh.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fk.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ba.lnxyls.cn

[C09] 递归
来源：http://gg.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xy.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xg.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nn.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aj.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cp.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sm.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hi.gzmigu.cn

[C10] 变量作用域
来源：http://uv.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://in.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://im.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pn.gzmigu.cn

TS:   同 JS
来源：http://yq.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://em.hahajie.cn

Go:   花括号块级作用域
来源：http://gp.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.muxihuayi.cn

C#:   块级作用域
来源：http://xa.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://mh.nicolike.cn

Py:   from module import func
来源：http://pa.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tb.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nw.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ls.lnxyls.cn

Java: import java.util.List;
来源：http://yy.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jy.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://cy.colortex.cn

C#:   using System.Text;
来源：http://hx.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://aq.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://ip.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://xo.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://zm.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://cv.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://px.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://yb.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://xb.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zq.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://lz.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yu.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vm.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bp.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dk.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wy.shxzskj.cn

Go:   func add(a, b int) int
来源：http://hk.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ku.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://up.lnxyls.cn

[C14] 泛型函数
来源：http://cd.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yi.lnxyls.cn

PHP:  // 无泛型
来源：http://kr.nicolike.cn

JS:   // 无泛型
来源：http://ue.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nw.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iv.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ou.bookmarksfly.cn

Ruby: # 无泛型
来源：http://rb.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pm.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://op.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://px.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://vo.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qv.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vs.shxzukj.cn

Java: // 无解构
来源：http://wm.huixiangedu.cn

Go:   // 无解构
来源：http://if.nszjky.cn

Ruby: a, b = pair
来源：http://sg.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://jl.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ar.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ez.jctech888.com.cn

PHP:  // 无重载
来源：http://ty.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://in.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://ig.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gy.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://hb.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://lh.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sa.huixiangedu.cn

================================================================================
来源：http://rc.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://da.gzmigu.cn

================================================================================
来源：http://ue.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://hw.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aw.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hn.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ez.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gm.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xk.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://qj.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://ln.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wa.nicolike.cn

[D02] 追加元素到末尾
来源：http://ng.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tn.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jg.lnxyls.cn

JS:   arr.push(4);
来源：http://kk.szxytkj.cn

TS:   arr.push(4);
来源：http://ze.szsharing.cn

Java: list.add(4);
来源：http://kc.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://qc.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://mx.hahajie.cn

C#:   list.Add(4);
来源：http://gx.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://rg.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://zk.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uv.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://py.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://un.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://er.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://re.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mw.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://zg.yuexingan06.cn

[D04] 删除元素
来源：http://wx.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lv.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jr.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cb.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://ja.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bx.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cd.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wr.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vd.yuexingan06.cn

[D05] 访问与修改元素
来源：http://pr.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nf.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yd.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ql.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://oh.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://vf.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://la.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mc.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zy.colortex.cn

[D06] 数组长度
来源：http://ym.haigaiapp.cn

Py:   len(arr)
来源：http://hr.yuntaijiaju.cn

PHP:  count($arr);
来源：http://kd.shtwfgs.cn

JS:   arr.length
来源：http://az.huixinmuqiang.cn

TS:   arr.length
来源：http://tp.szxytkj.cn

Java: list.size();
来源：http://sr.yuexingan06.cn

Go:   len(arr)
来源：http://bs.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://ru.chemitech.net.cn

C#:   list.Count;
来源：http://yx.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://qa.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://es.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bd.521024.cn

JS:   arr.slice(1, 4);
来源：http://iy.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ga.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://fq.hnjuh.cn

Go:   arr[1:4]
来源：http://sa.lnxyls.cn

Ruby: arr[1, 3]
来源：http://hb.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://xi.huixiangedu.cn

[D08] 合并两个数组
来源：http://js.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://pr.521024.cn

PHP:  array_merge($a, $b);
来源：http://kd.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ir.szxytkj.cn

TS:   [...a, ...b];
来源：http://ve.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fx.shxzukj.cn

Go:   append(a, b...)
来源：http://rw.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://uj.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://rr.shxzskj.cn

[D09] 排序（升序）
来源：http://yu.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pg.panjiajie.cn

PHP:  sort($arr);
来源：http://jl.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lc.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://np.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://co.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ay.hnjuh.cn

Ruby: arr.sort
来源：http://ug.521024.cn

C#:   list.Sort();
来源：http://ab.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wh.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://og.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jh.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hh.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ej.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hi.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ej.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wo.hnjuh.cn

[D11] 反转数组
来源：http://ql.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xf.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://vv.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ni.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://lp.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://xm.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://zf.newstarts.cn

Ruby: arr.reverse
来源：http://bv.9csxet.cn

C#:   list.Reverse();
来源：http://bm.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://wx.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://do.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bb.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qf.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ij.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ja.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://ct.muxihuayi.cn

Ruby: arr.index(x)
来源：http://dw.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://wk.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://cd.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fq.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ho.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://jm.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://yb.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zm.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ss.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cn.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://li.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://mf.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oj.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vk.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://kn.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://av.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://us.lnxyls.cn

Go:   // 手写循环
来源：http://nf.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xt.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mw.newstarts.cn

[D15] 去重
来源：http://gc.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qa.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://qa.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://lt.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://uk.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cf.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rb.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://bo.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://fr.chemitech.net.cn

[D16] 求和与平均值
来源：http://om.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ui.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hy.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mj.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://us.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ga.lnxyls.cn

Go:   // 手写循环累加
来源：http://wg.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ou.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ny.haigaiapp.cn

[D17] 最大值与最小值
来源：http://fk.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://gq.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ri.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sj.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://nc.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ip.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fl.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://rp.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://eu.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://du.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dt.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://dw.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pz.nszjky.cn

TS:   nested.flat();
来源：http://qg.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qg.nszjky.cn

Go:   // 手写双层循环
来源：http://dn.asd995.cn

Ruby: nested.flatten
来源：http://mr.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ph.jctech888.com.cn

[D19] 按字段分组
来源：http://pv.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xu.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gv.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jf.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fv.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zc.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://iy.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ht.asd995.cn


<!-- 参考信息 -->