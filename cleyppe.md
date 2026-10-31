代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vc.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jt.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wc.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://xf.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://up.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://se.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://eo.huixiangedu.cn

[C05] 返回多个值
来源：http://ib.jctech888.com.cn

Py:   return a, b
来源：http://cy.hahajie.cn

PHP:  return [$a, $b];
来源：http://ur.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rp.huanxung.cn

TS:   return { a, b };
来源：http://xl.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mt.newstarts.cn

Go:   return a, b
来源：http://pi.shxzukj.cn

Ruby: return a, b
来源：http://by.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://uq.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ww.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ya.huanxung.cn

JS:   const square = x => x * x;
来源：http://rg.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ro.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gl.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kr.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://zy.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hy.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ni.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mj.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uq.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sh.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://vg.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uf.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rk.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://sl.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kb.asd995.cn

[C08] 闭包
来源：http://gw.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xh.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iy.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yg.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fr.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sn.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://za.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ag.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qg.colortex.cn

[C09] 递归
来源：http://hf.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kb.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://on.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ho.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://is.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://px.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pe.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ue.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hb.hahajie.cn

[C10] 变量作用域
来源：http://qu.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ar.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qk.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ny.asd995.cn

TS:   同 JS
来源：http://tx.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ez.shtwfgs.cn

Go:   花括号块级作用域
来源：http://he.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ug.huanxung.cn

C#:   块级作用域
来源：http://wn.newstarts.cn

[C11] 模块导入与导出
来源：http://pv.chemitech.net.cn

Py:   from module import func
来源：http://hs.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pa.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sa.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pf.521024.cn

Java: import java.util.List;
来源：http://cy.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ut.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://nj.nicolike.cn

C#:   using System.Text;
来源：http://nz.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://ug.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://sg.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://qt.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://pc.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://cu.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pi.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://rf.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://gx.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ry.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://mr.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ga.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bw.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cr.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://cs.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zi.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jw.chemitech.net.cn

[C14] 泛型函数
来源：http://gy.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yj.haigaiapp.cn

PHP:  // 无泛型
来源：http://uy.bjjhwx.cn

JS:   // 无泛型
来源：http://rz.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://js.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ua.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dn.yuexingan06.cn

Ruby: # 无泛型
来源：http://uk.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fm.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://yq.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xq.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://mt.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.nszjky.cn

Java: // 无解构
来源：http://ws.shtwfgs.cn

Go:   // 无解构
来源：http://mu.huanxung.cn

Ruby: a, b = pair
来源：http://ut.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://ep.szsharing.cn

[C16] 函数 / 方法重载
来源：http://te.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://un.wgjwhj.cn

PHP:  // 无重载
来源：http://yi.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ra.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://xj.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gb.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://yo.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://ak.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://je.bookmarksfly.cn

================================================================================
来源：http://up.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://tn.chemitech.net.cn

================================================================================
来源：http://bp.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://kq.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mg.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vj.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xc.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xr.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mg.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ys.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://im.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ug.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://vr.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ra.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hg.lnxyls.cn

JS:   arr.push(4);
来源：http://iz.hahajie.cn

TS:   arr.push(4);
来源：http://zs.shtwfgs.cn

Java: list.add(4);
来源：http://ah.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://up.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://hs.hahajie.cn

C#:   list.Add(4);
来源：http://gs.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://pe.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://dx.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kw.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bd.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://xv.muxihuayi.cn

Java: list.add(0, 0);
来源：http://dj.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yp.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oe.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ly.bjjhwx.cn

[D04] 删除元素
来源：http://sm.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ut.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ro.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nz.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://in.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://py.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bi.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vg.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wz.huixiangedu.cn

[D05] 访问与修改元素
来源：http://oe.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ov.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fp.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iq.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ck.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://jo.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://dc.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rq.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vk.nszjky.cn

[D06] 数组长度
来源：http://so.521024.cn

Py:   len(arr)
来源：http://ya.bookmarksfly.cn

PHP:  count($arr);
来源：http://ri.huixiangedu.cn

JS:   arr.length
来源：http://nw.lnxyls.cn

TS:   arr.length
来源：http://dx.chemitech.net.cn

Java: list.size();
来源：http://ea.huixinmuqiang.cn

Go:   len(arr)
来源：http://qk.nszjky.cn

Ruby: arr.length; arr.size
来源：http://qb.bookmarksfly.cn

C#:   list.Count;
来源：http://mm.asd995.cn

[D07] 切片 / 取子数组
来源：http://di.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pm.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://om.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://bz.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://xo.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://zv.shtwfgs.cn

Go:   arr[1:4]
来源：http://qk.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://pu.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://ke.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ll.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://ya.colortex.cn

PHP:  array_merge($a, $b);
来源：http://mp.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tq.9csxet.cn

TS:   [...a, ...b];
来源：http://ka.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vi.jctech888.com.cn

Go:   append(a, b...)
来源：http://ty.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://hb.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://og.nszjky.cn

[D09] 排序（升序）
来源：http://qu.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://cd.panjiajie.cn

PHP:  sort($arr);
来源：http://mx.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://by.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sw.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qb.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ou.bjjhwx.cn

Ruby: arr.sort
来源：http://kf.bjjhwx.cn

C#:   list.Sort();
来源：http://ps.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rk.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jn.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kt.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gy.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nb.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tu.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sd.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oz.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://de.hahajie.cn

[D11] 反转数组
来源：http://ie.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://px.newstarts.cn

PHP:  array_reverse($arr);
来源：http://vd.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ko.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://qr.nicolike.cn

Java: Collections.reverse(list);
来源：http://ri.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://vx.yuexingan06.cn

Ruby: arr.reverse
来源：http://yk.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://pd.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://zl.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://tu.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hh.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ar.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dl.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pw.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://gs.lnxyls.cn

Ruby: arr.index(x)
来源：http://di.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://uz.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://fo.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rw.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://so.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://qt.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://ex.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rr.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vl.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ny.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wq.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://cx.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://to.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dl.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://mk.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://hi.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ff.muxihuayi.cn

Go:   // 手写循环
来源：http://qn.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mv.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rp.muxihuayi.cn

[D15] 去重
来源：http://qq.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lw.szsharing.cn

PHP:  array_unique($arr);
来源：http://mh.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://nc.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://co.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://as.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hg.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://uv.asd995.cn

C#:   list.Distinct().ToList()
来源：http://tt.newstarts.cn

[D16] 求和与平均值
来源：http://xh.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tj.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ws.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rx.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hk.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ec.gzmigu.cn

Go:   // 手写循环累加
来源：http://gp.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dx.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://xd.521024.cn

[D17] 最大值与最小值
来源：http://dl.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://qj.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://fy.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yy.521024.cn

TS:   Math.max(...arr);
来源：http://pc.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hv.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ib.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ln.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://ku.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://zs.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xh.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://gp.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cp.szsharing.cn

TS:   nested.flat();
来源：http://sz.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fr.521024.cn

Go:   // 手写双层循环
来源：http://rl.szxytkj.cn

Ruby: nested.flatten
来源：http://hr.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://df.szxytkj.cn

[D19] 按字段分组
来源：http://oq.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ht.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ks.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qh.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zx.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bs.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://qt.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vp.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wy.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://xe.lnxyls.cn

Py:   Counter(arr)
来源：http://tr.hahajie.cn

PHP:  array_count_values($arr);
来源：http://zx.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xx.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vk.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gy.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://vp.bjjhwx.cn

Ruby: arr.tally
来源：http://vw.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pn.hahajie.cn

[D21] 判断是否包含某元素
来源：http://pz.wgjwhj.cn

Py:   x in arr
来源：http://ig.yuntaijiaju.cn


<!-- 参考信息 -->