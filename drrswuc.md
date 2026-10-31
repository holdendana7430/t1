代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://as.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pv.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nf.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://ro.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://wh.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://xl.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://zq.huixinmuqiang.cn

[C05] 返回多个值
来源：http://rc.jianghongdianzi.cn

Py:   return a, b
来源：http://vk.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://dj.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ie.yuntaijiaju.cn

TS:   return { a, b };
来源：http://tr.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://as.jianghongdianzi.cn

Go:   return a, b
来源：http://pv.hahajie.cn

Ruby: return a, b
来源：http://ut.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://ia.asd995.cn

[C06] 匿名函数 / lambda
来源：http://qy.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://xb.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://od.colortex.cn

JS:   const square = x => x * x;
来源：http://tz.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://zs.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://la.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hp.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://hq.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qj.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://zy.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nl.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ro.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ag.muxihuayi.cn

TS:   arr.map(String)
来源：http://wr.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pw.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://so.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://vf.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gl.colortex.cn

[C08] 闭包
来源：http://ch.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ga.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vu.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aa.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rz.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lw.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wv.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nd.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dv.haigaiapp.cn

[C09] 递归
来源：http://kp.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ox.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wq.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pd.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pe.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bv.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cv.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kp.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xk.chemitech.net.cn

[C10] 变量作用域
来源：http://sn.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wo.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://am.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zm.huixinmuqiang.cn

TS:   同 JS
来源：http://ni.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://rf.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://pg.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://of.wgjwhj.cn

C#:   块级作用域
来源：http://el.szsharing.cn

[C11] 模块导入与导出
来源：http://vz.panjiajie.cn

Py:   from module import func
来源：http://sj.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ls.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pd.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zo.newstarts.cn

Java: import java.util.List;
来源：http://xs.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uq.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://ki.szxytkj.cn

C#:   using System.Text;
来源：http://dt.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://ou.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://fm.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://le.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://rn.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://bw.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fl.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ws.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://bs.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cz.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://tu.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ty.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mv.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ov.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ax.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pd.newstarts.cn

Go:   func add(a, b int) int
来源：http://tn.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ok.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pc.huixiangedu.cn

[C14] 泛型函数
来源：http://oa.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rq.521024.cn

PHP:  // 无泛型
来源：http://eu.9csxet.cn

JS:   // 无泛型
来源：http://hp.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ug.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fj.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xg.wgjwhj.cn

Ruby: # 无泛型
来源：http://sl.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ts.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://cf.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vj.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://vx.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ll.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kp.bookmarksfly.cn

Java: // 无解构
来源：http://az.9csxet.cn

Go:   // 无解构
来源：http://hp.nszjky.cn

Ruby: a, b = pair
来源：http://ii.nicolike.cn

C#:   var (a, b) = pair;
来源：http://ws.newstarts.cn

[C16] 函数 / 方法重载
来源：http://gl.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yn.colortex.cn

PHP:  // 无重载
来源：http://oe.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ip.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://ft.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://da.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://vh.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://wz.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hl.yuntaijiaju.cn

================================================================================
来源：http://vs.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://qp.colortex.cn

================================================================================
来源：http://bf.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://sw.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yt.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vd.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gv.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lq.chemitech.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fo.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://ra.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://pe.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jz.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ly.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bb.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sx.521024.cn

JS:   arr.push(4);
来源：http://rn.colortex.cn

TS:   arr.push(4);
来源：http://tk.yuntaijiaju.cn

Java: list.add(4);
来源：http://xc.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ws.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://kh.9csxet.cn

C#:   list.Add(4);
来源：http://gk.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://fy.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://er.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bs.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ja.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://il.szsharing.cn

Java: list.add(0, 0);
来源：http://xi.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qf.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bw.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://cz.huanxung.cn

[D04] 删除元素
来源：http://oe.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ul.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yi.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vl.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://iz.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kk.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jy.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yt.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zm.bjjhwx.cn

[D05] 访问与修改元素
来源：http://gn.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://io.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yq.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ox.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://go.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://vi.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kb.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yc.hnjuh.cn

[D06] 数组长度
来源：http://gn.bookmarksfly.cn

Py:   len(arr)
来源：http://ze.newstarts.cn

PHP:  count($arr);
来源：http://ze.chemitech.net.cn

JS:   arr.length
来源：http://cm.shxzukj.cn

TS:   arr.length
来源：http://qw.chemitech.net.cn

Java: list.size();
来源：http://ui.chemitech.net.cn

Go:   len(arr)
来源：http://cy.asd995.cn

Ruby: arr.length; arr.size
来源：http://cm.muxihuayi.cn

C#:   list.Count;
来源：http://zr.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ar.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hn.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://za.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://if.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://oj.shxzskj.cn

Java: list.subList(1, 4);
来源：http://gu.newstarts.cn

Go:   arr[1:4]
来源：http://ul.hahajie.cn

Ruby: arr[1, 3]
来源：http://wp.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://ix.huixiangedu.cn

[D08] 合并两个数组
来源：http://jh.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://rp.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://jt.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pb.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ov.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tx.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ga.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://zp.521024.cn

C#:   a.Concat(b).ToList()
来源：http://nw.szxytkj.cn

[D09] 排序（升序）
来源：http://ci.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://pk.panjiajie.cn

PHP:  sort($arr);
来源：http://ax.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qw.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mf.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cs.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kt.hnjuh.cn

Ruby: arr.sort
来源：http://ml.bjjhwx.cn

C#:   list.Sort();
来源：http://qe.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mh.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yi.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ae.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zz.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qo.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gm.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gr.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vi.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vd.hahajie.cn

[D11] 反转数组
来源：http://ve.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gz.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://dm.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tl.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ur.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://cl.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://lf.9csxet.cn

Ruby: arr.reverse
来源：http://co.gzmigu.cn

C#:   list.Reverse();
来源：http://pg.lnxyls.cn

[D12] 查找元素下标
来源：http://ei.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://nv.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lx.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sv.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fa.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dg.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ir.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://eh.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://fx.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://gs.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yc.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ce.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://kf.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://ud.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lv.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sj.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tv.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zx.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://el.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dd.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yv.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://kz.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://og.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zb.jctech888.com.cn

Go:   // 手写循环
来源：http://qu.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://go.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qy.colortex.cn

[D15] 去重
来源：http://fr.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rd.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://is.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://nm.huanxung.cn

TS:   [...new Set(arr)]
来源：http://fw.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ui.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mn.wgjwhj.cn

Ruby: arr.uniq
来源：http://fu.521024.cn

C#:   list.Distinct().ToList()
来源：http://mt.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ee.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ep.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fb.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gr.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ok.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mj.jctech888.com.cn

Go:   // 手写循环累加
来源：http://pb.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tt.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://cf.nszjky.cn

[D17] 最大值与最小值
来源：http://zd.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://or.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://wd.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pu.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://yl.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fi.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uz.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://gd.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ef.521024.cn

[D18] 扁平化嵌套数组
来源：http://zb.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nf.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ru.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bk.haigaiapp.cn

TS:   nested.flat();
来源：http://xp.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vh.wgjwhj.cn

Go:   // 手写双层循环
来源：http://nb.haigaiapp.cn

Ruby: nested.flatten
来源：http://gr.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kp.jianghongdianzi.cn

[D19] 按字段分组
来源：http://da.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://on.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yy.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yf.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lg.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://er.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://zr.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gl.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nx.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://fz.szxytkj.cn

Py:   Counter(arr)
来源：http://ck.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ap.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vk.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gs.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mf.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://es.521024.cn

Ruby: arr.tally
来源：http://dv.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fz.colortex.cn

[D21] 判断是否包含某元素
来源：http://ne.nicolike.cn

Py:   x in arr
来源：http://nr.shxzukj.cn


<!-- 参考信息 -->