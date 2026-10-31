代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sy.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://be.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vs.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nt.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bw.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kk.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://gt.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jj.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ev.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://da.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bb.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://yb.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://hk.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://pm.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ps.huixiangedu.cn

[C05] 返回多个值
来源：http://yi.szsharing.cn

Py:   return a, b
来源：http://zj.hahajie.cn

PHP:  return [$a, $b];
来源：http://ki.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dg.huanxung.cn

TS:   return { a, b };
来源：http://kr.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://za.newstarts.cn

Go:   return a, b
来源：http://rj.wgjwhj.cn

Ruby: return a, b
来源：http://gj.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://wb.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://wf.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://ux.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wi.nszjky.cn

JS:   const square = x => x * x;
来源：http://yg.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://gy.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vc.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yj.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://dg.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wu.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://wn.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tp.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://es.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sp.nszjky.cn

TS:   arr.map(String)
来源：http://xb.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ca.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://kb.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jw.hahajie.cn

[C08] 闭包
来源：http://zy.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ul.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ul.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ld.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ne.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lg.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fh.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ty.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hk.szxytkj.cn

[C09] 递归
来源：http://dn.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xx.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vt.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xp.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mr.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aw.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rj.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wy.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fc.yuexingan06.cn

[C10] 变量作用域
来源：http://ua.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rw.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qg.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mt.bookmarksfly.cn

TS:   同 JS
来源：http://qi.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://hc.panjiajie.cn

Go:   花括号块级作用域
来源：http://kj.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xu.bjjhwx.cn

C#:   块级作用域
来源：http://gi.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ib.szxytkj.cn

Py:   from module import func
来源：http://rw.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wh.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pu.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xg.jctech888.com.cn

Java: import java.util.List;
来源：http://xb.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://on.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://he.yuntaijiaju.cn

C#:   using System.Text;
来源：http://xt.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ei.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://md.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://da.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://ad.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://qd.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ac.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ac.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://vp.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ac.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://zc.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nv.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jm.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ix.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zv.gzmigu.cn

Go:   func add(a, b int) int
来源：http://lw.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ko.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wd.szxytkj.cn

[C14] 泛型函数
来源：http://sa.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rr.newstarts.cn

PHP:  // 无泛型
来源：http://lg.szxytkj.cn

JS:   // 无泛型
来源：http://np.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yy.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://du.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xe.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://eo.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zh.newstarts.cn

[C15] 解构 / 展开参数
来源：http://hi.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ru.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://yn.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zh.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ck.muxihuayi.cn

Java: // 无解构
来源：http://tq.huanxung.cn

Go:   // 无解构
来源：http://um.huanxung.cn

Ruby: a, b = pair
来源：http://qz.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://fx.nszjky.cn

[C16] 函数 / 方法重载
来源：http://rd.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wv.szxytkj.cn

PHP:  // 无重载
来源：http://yg.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lp.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://qv.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lj.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://xt.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://qj.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cl.colortex.cn

================================================================================
来源：http://ph.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://au.hahajie.cn

================================================================================
来源：http://bc.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://vi.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eq.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ag.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qa.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hl.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ni.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://vp.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://cs.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://we.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://gl.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kk.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ta.szxytkj.cn

JS:   arr.push(4);
来源：http://qs.521024.cn

TS:   arr.push(4);
来源：http://dr.hnjuh.cn

Java: list.add(4);
来源：http://qd.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://db.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://sw.wgjwhj.cn

C#:   list.Add(4);
来源：http://gy.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://pc.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://ns.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://su.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ii.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://ec.wgjwhj.cn

Java: list.add(0, 0);
来源：http://aj.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xc.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bz.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://ma.gzmigu.cn

[D04] 删除元素
来源：http://ki.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://js.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zy.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mf.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://zx.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cg.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kb.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://px.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bb.hahajie.cn

[D05] 访问与修改元素
来源：http://ro.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tm.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ae.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bb.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://ph.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zg.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ng.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://do.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xp.jianghongdianzi.cn

[D06] 数组长度
来源：http://fv.panjiajie.cn

Py:   len(arr)
来源：http://iu.newstarts.cn

PHP:  count($arr);
来源：http://nh.huixiangedu.cn

JS:   arr.length
来源：http://yx.panjiajie.cn

TS:   arr.length
来源：http://ji.haigaiapp.cn

Java: list.size();
来源：http://zp.shxzukj.cn

Go:   len(arr)
来源：http://wh.nicolike.cn

Ruby: arr.length; arr.size
来源：http://jk.huixinmuqiang.cn

C#:   list.Count;
来源：http://aj.521024.cn

[D07] 切片 / 取子数组
来源：http://yg.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rl.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://px.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://rj.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://qu.newstarts.cn

Java: list.subList(1, 4);
来源：http://le.asd995.cn

Go:   arr[1:4]
来源：http://ly.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zf.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://vi.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://re.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://fi.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://aj.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sy.panjiajie.cn

TS:   [...a, ...b];
来源：http://mi.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ax.jctech888.com.cn

Go:   append(a, b...)
来源：http://lj.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://lj.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://tp.panjiajie.cn

[D09] 排序（升序）
来源：http://xi.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://rv.newstarts.cn

PHP:  sort($arr);
来源：http://uv.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wj.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zl.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iv.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rz.colortex.cn

Ruby: arr.sort
来源：http://pm.jctech888.com.cn

C#:   list.Sort();
来源：http://tb.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jr.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cu.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bv.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sp.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hj.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tx.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rn.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jp.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nm.asd995.cn

[D11] 反转数组
来源：http://mg.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ld.newstarts.cn

PHP:  array_reverse($arr);
来源：http://jt.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rq.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://ns.gzmigu.cn

Java: Collections.reverse(list);
来源：http://yg.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://hj.9csxet.cn

Ruby: arr.reverse
来源：http://sv.huixiangedu.cn

C#:   list.Reverse();
来源：http://ag.newstarts.cn

[D12] 查找元素下标
来源：http://kc.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://mz.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jx.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jd.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oj.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ib.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://rj.wgjwhj.cn

Ruby: arr.index(x)
来源：http://kl.huanxung.cn

C#:   list.IndexOf(x);
来源：http://oe.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://ii.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://so.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qv.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://so.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ev.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://en.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ji.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hl.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mr.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://qy.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bt.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wn.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://jx.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ef.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://li.szxytkj.cn

Go:   // 手写循环
来源：http://bm.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kr.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uc.hahajie.cn

[D15] 去重
来源：http://dl.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://in.asd995.cn

PHP:  array_unique($arr);
来源：http://cv.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ye.newstarts.cn

TS:   [...new Set(arr)]
来源：http://eb.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yl.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://so.521024.cn

Ruby: arr.uniq
来源：http://iu.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://mm.lnxyls.cn

[D16] 求和与平均值
来源：http://rj.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ii.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ul.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ye.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fn.shxzukj.cn

Go:   // 手写循环累加
来源：http://hs.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ym.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://jy.nszjky.cn

[D17] 最大值与最小值
来源：http://uu.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://yx.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://pz.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xi.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://ra.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ui.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wz.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://vy.asd995.cn

C#:   list.Max();  list.Min()
来源：http://ce.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://uj.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nl.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://ea.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tb.lnxyls.cn

TS:   nested.flat();
来源：http://gr.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jn.wgjwhj.cn

Go:   // 手写双层循环
来源：http://eb.szxytkj.cn

Ruby: nested.flatten
来源：http://pe.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qg.yuntaijiaju.cn

[D19] 按字段分组
来源：http://si.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qo.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qr.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pb.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tr.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ti.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://dq.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ek.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://so.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://ai.gzmigu.cn

Py:   Counter(arr)
来源：http://ee.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://dj.yuexingan06.cn


<!-- 参考信息 -->