代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ej.newstarts.cn

Go:   return a, b
来源：http://ti.panjiajie.cn

Ruby: return a, b
来源：http://vn.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://yh.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://wz.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://sj.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ks.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://vp.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://ck.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fr.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nt.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://dy.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ps.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://jk.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://am.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sm.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lr.hnjuh.cn

TS:   arr.map(String)
来源：http://nl.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sa.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kx.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://aa.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://br.shxzukj.cn

[C08] 闭包
来源：http://jp.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cl.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hd.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xe.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ki.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://en.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xc.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fv.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bd.szxytkj.cn

[C09] 递归
来源：http://ro.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jt.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ug.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jt.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://it.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gh.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ic.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cv.newstarts.cn

[C10] 变量作用域
来源：http://sq.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cv.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gg.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hr.jctech888.com.cn

TS:   同 JS
来源：http://mu.gzmigu.cn

Java: 方法内为块级作用域
来源：http://qn.huanxung.cn

Go:   花括号块级作用域
来源：http://jr.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qh.yuexingan06.cn

C#:   块级作用域
来源：http://ft.asd995.cn

[C11] 模块导入与导出
来源：http://pq.jianghongdianzi.cn

Py:   from module import func
来源：http://xz.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uo.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ch.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bc.jctech888.com.cn

Java: import java.util.List;
来源：http://qq.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://km.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://vm.shtwfgs.cn

C#:   using System.Text;
来源：http://hw.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://lz.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://ky.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://hg.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://ix.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ld.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pg.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://qn.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://pv.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qm.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://be.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xr.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ig.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iw.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fo.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pk.szsharing.cn

Go:   func add(a, b int) int
来源：http://sd.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zu.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yj.shxzukj.cn

[C14] 泛型函数
来源：http://bp.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://na.asd995.cn

PHP:  // 无泛型
来源：http://fy.huixinmuqiang.cn

JS:   // 无泛型
来源：http://lf.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://on.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hm.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zl.nicolike.cn

Ruby: # 无泛型
来源：http://gn.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gq.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://jv.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qv.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://is.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dy.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://km.lnxyls.cn

Java: // 无解构
来源：http://eg.hnjuh.cn

Go:   // 无解构
来源：http://il.yuexingan06.cn

Ruby: a, b = pair
来源：http://kq.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ut.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://bn.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ib.lnxyls.cn

PHP:  // 无重载
来源：http://eb.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vo.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://wl.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uu.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ag.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://gm.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eh.asd995.cn

================================================================================
来源：http://lj.asd995.cn

D. 数组 / 列表 / 集合
来源：http://mx.yuntaijiaju.cn

================================================================================
来源：http://hc.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://bh.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oy.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ro.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lc.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dn.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rp.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ao.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ma.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jk.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://sr.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ug.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://db.panjiajie.cn

JS:   arr.push(4);
来源：http://vu.panjiajie.cn

TS:   arr.push(4);
来源：http://dm.huixinmuqiang.cn

Java: list.add(4);
来源：http://ny.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://fx.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://lx.gzmigu.cn

C#:   list.Add(4);
来源：http://nd.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://bu.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://ko.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hy.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://um.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://fw.szxytkj.cn

Java: list.add(0, 0);
来源：http://vz.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fg.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vy.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://hs.chemitech.net.cn

[D04] 删除元素
来源：http://tl.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://je.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fm.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://re.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://qo.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sj.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qq.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://we.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nq.szxytkj.cn

[D05] 访问与修改元素
来源：http://kd.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ze.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uo.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mc.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ei.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ga.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://br.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vf.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jf.shtwfgs.cn

[D06] 数组长度
来源：http://xc.chemitech.net.cn

Py:   len(arr)
来源：http://nx.wgjwhj.cn

PHP:  count($arr);
来源：http://uo.colortex.cn

JS:   arr.length
来源：http://ob.lnxyls.cn

TS:   arr.length
来源：http://pd.szxytkj.cn

Java: list.size();
来源：http://bg.colortex.cn

Go:   len(arr)
来源：http://ks.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://pd.bjjhwx.cn

C#:   list.Count;
来源：http://df.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://xz.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fj.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cj.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://bo.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://ow.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://fr.szxytkj.cn

Go:   arr[1:4]
来源：http://bo.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://qn.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://mz.bjjhwx.cn

[D08] 合并两个数组
来源：http://dp.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://lf.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://wo.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ol.nszjky.cn

TS:   [...a, ...b];
来源：http://kh.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jl.panjiajie.cn

Go:   append(a, b...)
来源：http://uk.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://tq.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://dg.gzmigu.cn

[D09] 排序（升序）
来源：http://zh.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://lk.chemitech.net.cn

PHP:  sort($arr);
来源：http://ov.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vu.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ti.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ko.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yc.muxihuayi.cn

Ruby: arr.sort
来源：http://st.panjiajie.cn

C#:   list.Sort();
来源：http://vb.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lz.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rh.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://re.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kv.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lv.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dl.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lj.huixinmuqiang.cn

[D11] 反转数组
来源：http://hc.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nv.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://wb.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ez.nszjky.cn

TS:   [...arr].reverse();
来源：http://sf.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://mj.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://uu.haigaiapp.cn

Ruby: arr.reverse
来源：http://ix.wgjwhj.cn

C#:   list.Reverse();
来源：http://vt.yuexingan06.cn

[D12] 查找元素下标
来源：http://od.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://wh.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vb.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dz.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ep.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eh.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://zb.shxzskj.cn

Ruby: arr.index(x)
来源：http://le.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://xw.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ms.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cd.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sg.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://so.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://is.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nw.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kt.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ai.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uh.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://pk.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fr.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://km.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://zm.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://em.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ec.wgjwhj.cn

Go:   // 手写循环
来源：http://ru.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hi.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://px.panjiajie.cn

[D15] 去重
来源：http://ba.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://js.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ux.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://sg.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://eg.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rs.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rv.9csxet.cn

Ruby: arr.uniq
来源：http://ye.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://lw.szxytkj.cn

[D16] 求和与平均值
来源：http://gh.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gw.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lh.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lu.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bp.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jy.bjjhwx.cn

Go:   // 手写循环累加
来源：http://rj.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yo.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://kt.muxihuayi.cn

[D17] 最大值与最小值
来源：http://ds.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://am.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://gp.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lv.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://is.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mp.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vl.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://lc.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://nj.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://mn.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dh.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://zg.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rx.haigaiapp.cn

TS:   nested.flat();
来源：http://je.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zv.asd995.cn

Go:   // 手写双层循环
来源：http://pt.nszjky.cn

Ruby: nested.flatten
来源：http://jg.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vh.nszjky.cn

[D19] 按字段分组
来源：http://yx.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oo.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gu.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://le.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://no.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vu.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://sg.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://en.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ws.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://yc.chemitech.net.cn

Py:   Counter(arr)
来源：http://yx.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ms.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ur.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://we.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://py.521024.cn

Go:   // 手写 map[T]int
来源：http://oo.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ym.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mr.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://fw.wgjwhj.cn

Py:   x in arr
来源：http://ed.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://ng.yuexingan06.cn

JS:   arr.includes(x)
来源：http://jw.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://qc.wgjwhj.cn

Java: list.contains(x)
来源：http://ra.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://dj.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://mc.shxzskj.cn

C#:   list.Contains(x)
来源：http://je.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://cr.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vp.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://li.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hl.bookmarksfly.cn

TS:   [...arr];
来源：http://as.szsharing.cn


<!-- 参考信息 -->