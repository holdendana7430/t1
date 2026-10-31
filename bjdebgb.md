代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://gu.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://oy.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://un.shxzskj.cn

[C05] 返回多个值
来源：http://he.hnjuh.cn

Py:   return a, b
来源：http://ay.shxzukj.cn

PHP:  return [$a, $b];
来源：http://jn.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ij.muxihuayi.cn

TS:   return { a, b };
来源：http://jf.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fd.huixiangedu.cn

Go:   return a, b
来源：http://eg.nszjky.cn

Ruby: return a, b
来源：http://qp.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://ax.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ax.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://vt.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kh.colortex.cn

JS:   const square = x => x * x;
来源：http://vp.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ou.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ag.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vp.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://mt.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ie.nicolike.cn

[C07] 把函数作为参数传入
来源：http://gm.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hb.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mp.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xe.521024.cn

TS:   arr.map(String)
来源：http://hv.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bi.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tt.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://zl.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ld.nicolike.cn

[C08] 闭包
来源：http://ic.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ac.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tu.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yq.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fm.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xa.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zh.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nd.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gu.shxzukj.cn

[C09] 递归
来源：http://wu.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oj.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tp.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lm.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lq.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fn.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kl.szxytkj.cn

[C10] 变量作用域
来源：http://kw.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zh.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wk.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tn.muxihuayi.cn

TS:   同 JS
来源：http://fp.hahajie.cn

Java: 方法内为块级作用域
来源：http://sk.521024.cn

Go:   花括号块级作用域
来源：http://qm.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ma.szxytkj.cn

C#:   块级作用域
来源：http://wj.bjjhwx.cn

[C11] 模块导入与导出
来源：http://jo.521024.cn

Py:   from module import func
来源：http://pu.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://re.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lp.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hs.muxihuayi.cn

Java: import java.util.List;
来源：http://dq.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xr.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://mu.9csxet.cn

C#:   using System.Text;
来源：http://qa.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://hw.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://qx.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://el.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://fh.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ip.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jw.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://hz.521024.cn

Ruby: -> { puts "run" }.call
来源：http://kb.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mq.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ca.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uy.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nl.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ef.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xp.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ch.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://yk.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ky.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mw.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ts.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oh.newstarts.cn

PHP:  // 无泛型
来源：http://si.shxzukj.cn

JS:   // 无泛型
来源：http://zg.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oy.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kf.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xx.gzmigu.cn

Ruby: # 无泛型
来源：http://ck.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mv.newstarts.cn

[C15] 解构 / 展开参数
来源：http://yi.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://er.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ln.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eo.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nu.huanxung.cn

Java: // 无解构
来源：http://dz.shxzukj.cn

Go:   // 无解构
来源：http://ep.521024.cn

Ruby: a, b = pair
来源：http://rz.nicolike.cn

C#:   var (a, b) = pair;
来源：http://mu.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://fb.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yq.newstarts.cn

PHP:  // 无重载
来源：http://ti.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cn.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ml.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gk.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://hp.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://af.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ko.newstarts.cn

================================================================================
来源：http://xm.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://ym.panjiajie.cn

================================================================================
来源：http://xf.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://wc.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qm.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yc.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yn.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vx.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jt.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ae.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://md.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://su.nszjky.cn

[D02] 追加元素到末尾
来源：http://nz.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cq.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tb.shxzskj.cn

JS:   arr.push(4);
来源：http://vc.shxzukj.cn

TS:   arr.push(4);
来源：http://wg.chemitech.net.cn

Java: list.add(4);
来源：http://gi.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ej.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ty.panjiajie.cn

C#:   list.Add(4);
来源：http://fv.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://mv.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://uv.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ei.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rx.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://fg.colortex.cn

Java: list.add(0, 0);
来源：http://zd.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jg.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ql.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://qg.yuntaijiaju.cn

[D04] 删除元素
来源：http://rk.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pw.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sk.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ig.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ne.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://er.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://de.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ux.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ru.hnjuh.cn

[D05] 访问与修改元素
来源：http://nl.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://az.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aj.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kx.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://yj.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://zw.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://uk.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://za.panjiajie.cn

[D06] 数组长度
来源：http://ze.szxytkj.cn

Py:   len(arr)
来源：http://cu.nicolike.cn

PHP:  count($arr);
来源：http://di.huanxung.cn

JS:   arr.length
来源：http://ve.huanxung.cn

TS:   arr.length
来源：http://tz.panjiajie.cn

Java: list.size();
来源：http://mm.bookmarksfly.cn

Go:   len(arr)
来源：http://gb.nicolike.cn

Ruby: arr.length; arr.size
来源：http://kc.521024.cn

C#:   list.Count;
来源：http://sj.nszjky.cn

[D07] 切片 / 取子数组
来源：http://wo.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dt.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cb.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://lk.asd995.cn

TS:   arr.slice(1, 4);
来源：http://sa.521024.cn

Java: list.subList(1, 4);
来源：http://er.shxzukj.cn

Go:   arr[1:4]
来源：http://kb.521024.cn

Ruby: arr[1, 3]
来源：http://qb.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ks.szxytkj.cn

[D08] 合并两个数组
来源：http://ul.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://wr.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://bw.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fp.panjiajie.cn

TS:   [...a, ...b];
来源：http://bp.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ku.szxytkj.cn

Go:   append(a, b...)
来源：http://qv.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://lo.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://jt.jctech888.com.cn

[D09] 排序（升序）
来源：http://ql.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://wa.jctech888.com.cn

PHP:  sort($arr);
来源：http://eb.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ri.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://do.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://je.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sm.huanxung.cn

Ruby: arr.sort
来源：http://jv.muxihuayi.cn

C#:   list.Sort();
来源：http://ws.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xf.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jr.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ra.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://my.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jb.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ps.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dq.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ya.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cq.yuntaijiaju.cn

[D11] 反转数组
来源：http://ut.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://op.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://dj.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qs.szxytkj.cn

TS:   [...arr].reverse();
来源：http://di.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://yu.colortex.cn

Go:   slices.Reverse(arr)
来源：http://wj.huixiangedu.cn

Ruby: arr.reverse
来源：http://ox.nszjky.cn

C#:   list.Reverse();
来源：http://eq.hahajie.cn

[D12] 查找元素下标
来源：http://eo.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://wb.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iw.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bf.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jg.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tk.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://tv.lnxyls.cn

Ruby: arr.index(x)
来源：http://ov.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://ag.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ke.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zp.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uf.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://cr.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://yf.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aa.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vw.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jk.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rw.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://yw.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://je.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sw.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://lk.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://dq.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ct.521024.cn

Go:   // 手写循环
来源：http://fg.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qe.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hu.gzmigu.cn

[D15] 去重
来源：http://gt.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ip.hahajie.cn

PHP:  array_unique($arr);
来源：http://zl.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://vc.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://zq.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ew.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rx.colortex.cn

Ruby: arr.uniq
来源：http://gt.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://zf.nszjky.cn

[D16] 求和与平均值
来源：http://vj.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pl.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fz.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nz.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xe.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fh.szsharing.cn

Go:   // 手写循环累加
来源：http://mk.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mg.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://ov.asd995.cn

[D17] 最大值与最小值
来源：http://hy.521024.cn

Py:   max(arr);  min(arr)
来源：http://me.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://nl.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vq.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ix.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://um.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hp.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://ut.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://pa.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://oi.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mx.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://gz.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qm.yuexingan06.cn

TS:   nested.flat();
来源：http://pe.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yv.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ke.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://wt.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wj.nszjky.cn

[D19] 按字段分组
来源：http://gd.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://am.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qe.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mf.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ho.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gv.asd995.cn

Go:   // 手写 map[string][]T
来源：http://qn.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tl.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rd.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://cy.shtwfgs.cn

Py:   Counter(arr)
来源：http://jv.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://nk.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kp.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ar.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ft.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://rg.jctech888.com.cn

Ruby: arr.tally
来源：http://gn.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pn.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://xf.9csxet.cn

Py:   x in arr
来源：http://er.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://wb.shxzukj.cn

JS:   arr.includes(x)
来源：http://vi.521024.cn

TS:   arr.includes(x)
来源：http://ko.hahajie.cn

Java: list.contains(x)
来源：http://hh.jianghongdianzi.cn


<!-- 参考信息 -->