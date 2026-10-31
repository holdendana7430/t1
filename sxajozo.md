代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://ek.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://yj.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://nh.shtwfgs.cn

[C05] 返回多个值
来源：http://sh.haigaiapp.cn

Py:   return a, b
来源：http://sx.szsharing.cn

PHP:  return [$a, $b];
来源：http://dh.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vn.hnjuh.cn

TS:   return { a, b };
来源：http://vq.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tk.chemitech.net.cn

Go:   return a, b
来源：http://os.wgjwhj.cn

Ruby: return a, b
来源：http://os.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://rz.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://rs.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ib.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ed.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://yg.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://mc.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qx.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gn.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://oi.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xs.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://cy.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gm.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fh.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://io.521024.cn

TS:   arr.map(String)
来源：http://xk.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://of.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cp.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://qb.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oq.huanxung.cn

[C08] 闭包
来源：http://py.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://an.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fd.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zj.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://df.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hq.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rc.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xt.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uu.huanxung.cn

[C09] 递归
来源：http://gr.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kh.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bi.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ed.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lh.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xs.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ny.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hq.nszjky.cn

[C10] 变量作用域
来源：http://ni.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hj.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hb.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sf.yuntaijiaju.cn

TS:   同 JS
来源：http://jb.huanxung.cn

Java: 方法内为块级作用域
来源：http://fl.szsharing.cn

Go:   花括号块级作用域
来源：http://vp.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ei.jctech888.com.cn

C#:   块级作用域
来源：http://he.shtwfgs.cn

[C11] 模块导入与导出
来源：http://sx.jianghongdianzi.cn

Py:   from module import func
来源：http://eq.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nc.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hd.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://re.chemitech.net.cn

Java: import java.util.List;
来源：http://xy.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uu.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://sq.muxihuayi.cn

C#:   using System.Text;
来源：http://fp.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://oq.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ob.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://vt.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://lt.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ch.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dh.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://mg.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://it.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vg.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://in.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tr.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ab.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aa.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://td.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bn.panjiajie.cn

Go:   func add(a, b int) int
来源：http://tl.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://li.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fw.gzmigu.cn

[C14] 泛型函数
来源：http://bk.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ux.haigaiapp.cn

PHP:  // 无泛型
来源：http://wo.newstarts.cn

JS:   // 无泛型
来源：http://gl.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zo.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://no.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://om.nicolike.cn

Ruby: # 无泛型
来源：http://lq.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eu.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://tn.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jj.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://my.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://si.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ak.lnxyls.cn

Java: // 无解构
来源：http://ey.wgjwhj.cn

Go:   // 无解构
来源：http://jn.9csxet.cn

Ruby: a, b = pair
来源：http://yb.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://po.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ze.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kp.jianghongdianzi.cn

PHP:  // 无重载
来源：http://xi.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hu.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://la.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xe.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ty.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://sm.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yf.shxzukj.cn

================================================================================
来源：http://wj.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://am.jctech888.com.cn

================================================================================
来源：http://vh.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://oo.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ct.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mm.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pr.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ag.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pc.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://jg.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://fu.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xk.nicolike.cn

[D02] 追加元素到末尾
来源：http://aa.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ru.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fq.wgjwhj.cn

JS:   arr.push(4);
来源：http://fb.shtwfgs.cn

TS:   arr.push(4);
来源：http://zz.bjjhwx.cn

Java: list.add(4);
来源：http://or.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://mk.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://zf.hahajie.cn

C#:   list.Add(4);
来源：http://yi.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://np.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://sj.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wd.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tq.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://qa.gzmigu.cn

Java: list.add(0, 0);
来源：http://jb.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wv.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rl.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://xn.9csxet.cn

[D04] 删除元素
来源：http://qw.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nk.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tu.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vs.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://na.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cb.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wm.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gi.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://xr.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ng.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dv.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zo.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://qe.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://ah.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://rw.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jd.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qs.muxihuayi.cn

[D06] 数组长度
来源：http://hf.yuntaijiaju.cn

Py:   len(arr)
来源：http://xs.chemitech.net.cn

PHP:  count($arr);
来源：http://ik.nszjky.cn

JS:   arr.length
来源：http://ro.huixiangedu.cn

TS:   arr.length
来源：http://un.wgjwhj.cn

Java: list.size();
来源：http://om.asd995.cn

Go:   len(arr)
来源：http://nc.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://fn.shtwfgs.cn

C#:   list.Count;
来源：http://qz.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://ci.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jl.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vu.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://tr.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://le.nszjky.cn

Java: list.subList(1, 4);
来源：http://or.nszjky.cn

Go:   arr[1:4]
来源：http://vq.newstarts.cn

Ruby: arr[1, 3]
来源：http://zo.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://cz.colortex.cn

[D08] 合并两个数组
来源：http://gm.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://kp.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://bk.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zp.colortex.cn

TS:   [...a, ...b];
来源：http://tw.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cl.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://ru.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://eu.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ma.huanxung.cn

[D09] 排序（升序）
来源：http://zn.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://re.huanxung.cn

PHP:  sort($arr);
来源：http://rp.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gk.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ey.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ls.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zr.yuexingan06.cn

Ruby: arr.sort
来源：http://qq.hahajie.cn

C#:   list.Sort();
来源：http://el.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jw.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ej.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uk.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://km.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bo.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vm.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cp.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bg.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xn.bjjhwx.cn

[D11] 反转数组
来源：http://zb.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bx.colortex.cn

PHP:  array_reverse($arr);
来源：http://qm.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xh.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://yp.lnxyls.cn

Java: Collections.reverse(list);
来源：http://en.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://ii.asd995.cn

Ruby: arr.reverse
来源：http://cn.9csxet.cn

C#:   list.Reverse();
来源：http://us.lnxyls.cn

[D12] 查找元素下标
来源：http://bq.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://pc.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qe.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sr.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hb.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dg.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://de.yuexingan06.cn

Ruby: arr.index(x)
来源：http://rl.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://uz.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://xj.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mi.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ft.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://is.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://uw.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iq.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vi.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pm.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://xp.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oo.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ip.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ne.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://uk.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wp.jianghongdianzi.cn

Go:   // 手写循环
来源：http://be.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ty.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tv.huixiangedu.cn

[D15] 去重
来源：http://og.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.panjiajie.cn

PHP:  array_unique($arr);
来源：http://fd.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://as.huanxung.cn

TS:   [...new Set(arr)]
来源：http://mv.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jt.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qe.jctech888.com.cn

Ruby: arr.uniq
来源：http://yh.colortex.cn

C#:   list.Distinct().ToList()
来源：http://ny.szxytkj.cn

[D16] 求和与平均值
来源：http://rk.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jw.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bb.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://in.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ri.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jm.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://vy.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yp.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://fa.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://kg.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://rb.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://je.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pz.hahajie.cn

TS:   Math.max(...arr);
来源：http://id.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://px.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mi.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://gs.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://rh.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://yf.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qn.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://gm.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xn.haigaiapp.cn

TS:   nested.flat();
来源：http://gc.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ky.gzmigu.cn

Go:   // 手写双层循环
来源：http://yk.9csxet.cn

Ruby: nested.flatten
来源：http://yz.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yd.9csxet.cn

[D19] 按字段分组
来源：http://bk.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uj.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mq.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mf.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mg.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zt.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://hy.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fq.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ip.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://hs.muxihuayi.cn

Py:   Counter(arr)
来源：http://wt.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://jl.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gx.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vq.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://md.newstarts.cn

Go:   // 手写 map[T]int
来源：http://mo.asd995.cn

Ruby: arr.tally
来源：http://by.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://jm.szxytkj.cn

Py:   x in arr
来源：http://uy.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://kg.wgjwhj.cn

JS:   arr.includes(x)
来源：http://st.szsharing.cn

TS:   arr.includes(x)
来源：http://nb.huixiangedu.cn

Java: list.contains(x)
来源：http://ij.huanxung.cn


<!-- 参考信息 -->