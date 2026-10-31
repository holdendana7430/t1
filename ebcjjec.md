代发 wailian999

Py:   return a, b
来源：http://qt.szsharing.cn

PHP:  return [$a, $b];
来源：http://im.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ti.hnjuh.cn

TS:   return { a, b };
来源：http://ma.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wa.szsharing.cn

Go:   return a, b
来源：http://xc.shtwfgs.cn

Ruby: return a, b
来源：http://th.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ib.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://go.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://nl.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kw.hnjuh.cn

JS:   const square = x => x * x;
来源：http://ae.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://gv.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ju.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ll.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ng.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pr.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://mm.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vd.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lw.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ye.hahajie.cn

TS:   arr.map(String)
来源：http://hn.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xe.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://os.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://oa.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zq.521024.cn

[C08] 闭包
来源：http://yz.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qx.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://if.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vq.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vh.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cl.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ev.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vv.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tx.huanxung.cn

[C09] 递归
来源：http://ke.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ic.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dn.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oh.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gi.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pq.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bw.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cn.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ho.hnjuh.cn

[C10] 变量作用域
来源：http://ps.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qc.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vz.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yw.muxihuayi.cn

TS:   同 JS
来源：http://yo.huanxung.cn

Java: 方法内为块级作用域
来源：http://ly.chemitech.net.cn

Go:   花括号块级作用域
来源：http://zc.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xo.jctech888.com.cn

C#:   块级作用域
来源：http://ka.nszjky.cn

[C11] 模块导入与导出
来源：http://gu.huixinmuqiang.cn

Py:   from module import func
来源：http://qr.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ha.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://od.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fl.shxzukj.cn

Java: import java.util.List;
来源：http://rl.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ma.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://pq.shtwfgs.cn

C#:   using System.Text;
来源：http://fx.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://bk.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://bv.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://zq.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ak.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://dt.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pl.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ui.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://bv.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ir.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://hi.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://te.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ny.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jb.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yl.lnxyls.cn

Go:   func add(a, b int) int
来源：http://tq.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hn.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ep.shtwfgs.cn

[C14] 泛型函数
来源：http://kd.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://km.haigaiapp.cn

PHP:  // 无泛型
来源：http://iu.yuntaijiaju.cn

JS:   // 无泛型
来源：http://wu.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://op.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hs.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vu.bjjhwx.cn

Ruby: # 无泛型
来源：http://fe.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://by.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://am.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cn.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://sj.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://io.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uc.huanxung.cn

Java: // 无解构
来源：http://ds.asd995.cn

Go:   // 无解构
来源：http://wp.wgjwhj.cn

Ruby: a, b = pair
来源：http://ay.huanxung.cn

C#:   var (a, b) = pair;
来源：http://iv.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ht.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ev.lnxyls.cn

PHP:  // 无重载
来源：http://qv.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oc.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nf.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://up.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://me.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zq.panjiajie.cn

================================================================================
来源：http://oi.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://pl.huixiangedu.cn

================================================================================
来源：http://ly.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ne.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zl.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sg.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://en.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ga.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nj.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://za.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ut.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lp.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://dw.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hh.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ni.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ui.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://tp.bjjhwx.cn

Java: list.add(4);
来源：http://zt.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://xt.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://so.muxihuayi.cn

C#:   list.Add(4);
来源：http://dx.asd995.cn

[D03] 在指定位置插入元素
来源：http://wy.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://ct.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dv.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pg.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://rw.colortex.cn

Java: list.add(0, 0);
来源：http://mv.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ak.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yq.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://ky.szsharing.cn

[D04] 删除元素
来源：http://vx.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yx.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zk.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://os.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://uo.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eb.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://li.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jj.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ul.shxzukj.cn

[D05] 访问与修改元素
来源：http://sv.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ay.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nn.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yq.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://lt.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://tw.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://eo.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tt.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ht.yuexingan06.cn

[D06] 数组长度
来源：http://zt.newstarts.cn

Py:   len(arr)
来源：http://js.521024.cn

PHP:  count($arr);
来源：http://px.9csxet.cn

JS:   arr.length
来源：http://si.chemitech.net.cn

TS:   arr.length
来源：http://pq.panjiajie.cn

Java: list.size();
来源：http://nv.shxzukj.cn

Go:   len(arr)
来源：http://bp.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://qc.muxihuayi.cn

C#:   list.Count;
来源：http://si.nszjky.cn

[D07] 切片 / 取子数组
来源：http://qg.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hp.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bd.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://eg.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://il.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://kh.gzmigu.cn

Go:   arr[1:4]
来源：http://hy.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://pr.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://ax.nszjky.cn

[D08] 合并两个数组
来源：http://zw.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://zj.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://zx.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rw.521024.cn

TS:   [...a, ...b];
来源：http://qc.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fm.shtwfgs.cn

Go:   append(a, b...)
来源：http://gt.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://em.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://xi.shxzukj.cn

[D09] 排序（升序）
来源：http://pb.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ul.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://zm.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qg.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ht.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sh.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xj.hahajie.cn

Ruby: arr.sort
来源：http://bk.521024.cn

C#:   list.Sort();
来源：http://au.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ea.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xq.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wb.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jb.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ns.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kj.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gz.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zo.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eh.szxytkj.cn

[D11] 反转数组
来源：http://qf.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oo.newstarts.cn

PHP:  array_reverse($arr);
来源：http://db.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ho.colortex.cn

TS:   [...arr].reverse();
来源：http://pf.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ka.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://dg.panjiajie.cn

Ruby: arr.reverse
来源：http://fq.bjjhwx.cn

C#:   list.Reverse();
来源：http://xh.hahajie.cn

[D12] 查找元素下标
来源：http://pe.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://jd.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rk.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xw.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zg.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vv.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://pw.521024.cn

Ruby: arr.index(x)
来源：http://ng.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://mz.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://be.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rv.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vm.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://vu.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://xh.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ej.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://no.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ud.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nv.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://qn.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://up.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xy.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://qq.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://ng.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oo.nszjky.cn

Go:   // 手写循环
来源：http://bu.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pd.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qh.colortex.cn

[D15] 去重
来源：http://al.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vc.szxytkj.cn

PHP:  array_unique($arr);
来源：http://qb.nicolike.cn

JS:   [...new Set(arr)]
来源：http://ck.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://fp.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zf.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mh.chemitech.net.cn

Ruby: arr.uniq
来源：http://ae.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://nl.bookmarksfly.cn

[D16] 求和与平均值
来源：http://qp.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lt.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pe.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jo.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qv.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://fo.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kr.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://do.muxihuayi.cn

[D17] 最大值与最小值
来源：http://ev.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://qh.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://kg.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://px.nszjky.cn

TS:   Math.max(...arr);
来源：http://qz.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gh.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yf.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://td.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://fd.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://an.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wz.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://jv.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lw.shxzskj.cn

TS:   nested.flat();
来源：http://jj.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mc.newstarts.cn

Go:   // 手写双层循环
来源：http://rx.bookmarksfly.cn

Ruby: nested.flatten
来源：http://nn.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hp.shxzskj.cn

[D19] 按字段分组
来源：http://rc.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://go.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vg.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mt.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zg.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jl.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://dn.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ga.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mi.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://ta.wgjwhj.cn

Py:   Counter(arr)
来源：http://fo.newstarts.cn

PHP:  array_count_values($arr);
来源：http://lz.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fe.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wm.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bk.521024.cn

Go:   // 手写 map[T]int
来源：http://iu.colortex.cn

Ruby: arr.tally
来源：http://uh.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uq.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://jv.nszjky.cn

Py:   x in arr
来源：http://bl.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://xa.newstarts.cn

JS:   arr.includes(x)
来源：http://dz.wgjwhj.cn

TS:   arr.includes(x)
来源：http://vc.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ik.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://zm.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://fd.nszjky.cn

C#:   list.Contains(x)
来源：http://xb.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://af.szxytkj.cn


<!-- 参考信息 -->