代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://am.huixinmuqiang.cn

[C03] 可变参数
来源：http://xz.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://cx.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://im.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ny.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ww.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vu.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gd.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://vo.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uw.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ec.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nt.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jh.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://cq.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://yn.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://qx.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://pz.nszjky.cn

[C05] 返回多个值
来源：http://mn.haigaiapp.cn

Py:   return a, b
来源：http://le.hahajie.cn

PHP:  return [$a, $b];
来源：http://sv.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uz.bjjhwx.cn

TS:   return { a, b };
来源：http://kk.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qq.szsharing.cn

Go:   return a, b
来源：http://kc.bjjhwx.cn

Ruby: return a, b
来源：http://wg.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://to.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://hp.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://pe.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fk.9csxet.cn

JS:   const square = x => x * x;
来源：http://ta.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://xp.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gh.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hs.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ca.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fd.hahajie.cn

[C07] 把函数作为参数传入
来源：http://xp.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zi.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://os.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ej.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://ek.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zg.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uk.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://xx.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iv.gzmigu.cn

[C08] 闭包
来源：http://wu.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://in.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bq.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fz.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rc.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uj.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jq.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hr.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lc.huixinmuqiang.cn

[C09] 递归
来源：http://ic.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eo.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gl.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ef.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://be.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nw.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wd.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wj.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://do.panjiajie.cn

[C10] 变量作用域
来源：http://jt.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://th.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uo.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bh.chemitech.net.cn

TS:   同 JS
来源：http://eu.szsharing.cn

Java: 方法内为块级作用域
来源：http://dg.huanxung.cn

Go:   花括号块级作用域
来源：http://as.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pe.shxzskj.cn

C#:   块级作用域
来源：http://su.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://au.yuexingan06.cn

Py:   from module import func
来源：http://zb.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fa.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://so.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xj.bjjhwx.cn

Java: import java.util.List;
来源：http://kr.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nl.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://gd.nicolike.cn

C#:   using System.Text;
来源：http://cm.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://jp.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://zy.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://qb.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ot.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://nl.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ok.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://kh.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://tv.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ou.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://lp.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mi.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wr.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ra.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wr.521024.cn

Go:   func add(a, b int) int
来源：http://oq.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qo.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ww.shxzskj.cn

[C14] 泛型函数
来源：http://ig.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ln.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://sb.bjjhwx.cn

JS:   // 无泛型
来源：http://fs.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://st.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bx.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qa.hnjuh.cn

Ruby: # 无泛型
来源：http://jv.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kw.hahajie.cn

[C15] 解构 / 展开参数
来源：http://pv.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ns.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://bl.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yx.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bm.bookmarksfly.cn

Java: // 无解构
来源：http://kj.bookmarksfly.cn

Go:   // 无解构
来源：http://rv.colortex.cn

Ruby: a, b = pair
来源：http://fe.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://vt.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://cv.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cd.szxytkj.cn

PHP:  // 无重载
来源：http://cm.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bm.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://yf.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ac.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://ow.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://ir.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bw.shxzukj.cn

================================================================================
来源：http://hr.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://oq.nszjky.cn

================================================================================
来源：http://ac.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://id.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qf.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gq.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://an.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lu.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xd.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://ow.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://sh.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vc.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://cr.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sb.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lc.szsharing.cn

JS:   arr.push(4);
来源：http://ev.shxzskj.cn

TS:   arr.push(4);
来源：http://al.huanxung.cn

Java: list.add(4);
来源：http://hb.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://er.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://se.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://sa.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://gs.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://yj.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qb.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vp.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://gp.bjjhwx.cn

Java: list.add(0, 0);
来源：http://az.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gt.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nu.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://rg.chemitech.net.cn

[D04] 删除元素
来源：http://hl.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sr.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ai.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uu.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://sj.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ga.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mn.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uk.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sl.hnjuh.cn

[D05] 访问与修改元素
来源：http://pu.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cz.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zs.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qi.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://xb.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://yd.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pz.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zv.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xq.shtwfgs.cn

[D06] 数组长度
来源：http://no.bjjhwx.cn

Py:   len(arr)
来源：http://nk.szsharing.cn

PHP:  count($arr);
来源：http://ua.colortex.cn

JS:   arr.length
来源：http://fi.yuexingan06.cn

TS:   arr.length
来源：http://gd.hahajie.cn

Java: list.size();
来源：http://ge.nicolike.cn

Go:   len(arr)
来源：http://ts.521024.cn

Ruby: arr.length; arr.size
来源：http://hp.szxytkj.cn

C#:   list.Count;
来源：http://kn.nicolike.cn

[D07] 切片 / 取子数组
来源：http://rm.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ka.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xp.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://pn.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ey.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://ca.hnjuh.cn

Go:   arr[1:4]
来源：http://pr.colortex.cn

Ruby: arr[1, 3]
来源：http://ha.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://by.hahajie.cn

[D08] 合并两个数组
来源：http://xs.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://ho.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://jk.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://af.asd995.cn

TS:   [...a, ...b];
来源：http://lj.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kx.asd995.cn

Go:   append(a, b...)
来源：http://ic.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://pl.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://ca.szsharing.cn

[D09] 排序（升序）
来源：http://jx.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://si.bjjhwx.cn

PHP:  sort($arr);
来源：http://gl.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sr.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wd.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fe.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xf.panjiajie.cn

Ruby: arr.sort
来源：http://kf.haigaiapp.cn

C#:   list.Sort();
来源：http://uf.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xf.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ww.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qu.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yq.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aq.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jo.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vh.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://od.bjjhwx.cn

[D11] 反转数组
来源：http://fr.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sq.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://ym.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nl.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://qm.hahajie.cn

Java: Collections.reverse(list);
来源：http://gj.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://vk.muxihuayi.cn

Ruby: arr.reverse
来源：http://ja.panjiajie.cn

C#:   list.Reverse();
来源：http://fj.jctech888.com.cn

[D12] 查找元素下标
来源：http://xr.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://ns.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pg.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://of.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tv.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mm.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://by.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://zn.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ky.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://tr.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yp.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://vh.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://et.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bh.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cr.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mz.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gf.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ei.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hu.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ga.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://bt.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://zq.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fi.nszjky.cn

Go:   // 手写循环
来源：http://ll.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tm.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ic.huanxung.cn

[D15] 去重
来源：http://sl.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ur.shxzukj.cn

PHP:  array_unique($arr);
来源：http://qg.huanxung.cn

JS:   [...new Set(arr)]
来源：http://cx.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ct.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sl.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xc.shxzskj.cn

Ruby: arr.uniq
来源：http://kl.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://di.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://yi.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nr.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fl.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bl.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ed.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uj.shtwfgs.cn

Go:   // 手写循环累加
来源：http://ft.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ph.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ha.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ja.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://eu.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://iw.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ef.shxzskj.cn

TS:   Math.max(...arr);
来源：http://gu.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fb.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cy.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://gk.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://yc.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://uq.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://do.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://oo.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xl.yuexingan06.cn

TS:   nested.flat();
来源：http://jl.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nv.asd995.cn

Go:   // 手写双层循环
来源：http://bj.huanxung.cn

Ruby: nested.flatten
来源：http://dj.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zr.jianghongdianzi.cn

[D19] 按字段分组
来源：http://xp.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ip.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tb.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yo.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qz.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oj.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://em.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vu.bookmarksfly.cn


<!-- 参考信息 -->