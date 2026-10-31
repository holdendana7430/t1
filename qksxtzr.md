代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://gm.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://vg.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://wb.nicolike.cn

[C05] 返回多个值
来源：http://ev.szsharing.cn

Py:   return a, b
来源：http://aw.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ly.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jq.chemitech.net.cn

TS:   return { a, b };
来源：http://zq.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zg.gzmigu.cn

Go:   return a, b
来源：http://ew.muxihuayi.cn

Ruby: return a, b
来源：http://wz.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://bc.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://aq.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://jf.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://et.lnxyls.cn

JS:   const square = x => x * x;
来源：http://az.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://lj.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jy.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bk.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://gb.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://os.szsharing.cn

[C07] 把函数作为参数传入
来源：http://mq.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hm.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aw.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cn.chemitech.net.cn

TS:   arr.map(String)
来源：http://ts.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ds.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fv.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://vi.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gi.muxihuayi.cn

[C08] 闭包
来源：http://as.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gk.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rd.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vl.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hj.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xf.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wb.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qx.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vq.shxzukj.cn

[C09] 递归
来源：http://au.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://en.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gr.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sz.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bw.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://on.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pv.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ql.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fw.newstarts.cn

[C10] 变量作用域
来源：http://xg.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://df.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://at.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kr.yuntaijiaju.cn

TS:   同 JS
来源：http://ti.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://op.szxytkj.cn

Go:   花括号块级作用域
来源：http://ed.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ax.huanxung.cn

C#:   块级作用域
来源：http://pb.bjjhwx.cn

[C11] 模块导入与导出
来源：http://aj.wgjwhj.cn

Py:   from module import func
来源：http://vc.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vf.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pq.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fw.yuexingan06.cn

Java: import java.util.List;
来源：http://xg.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vz.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ch.yuexingan06.cn

C#:   using System.Text;
来源：http://gp.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://au.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://if.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://fi.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ih.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://vh.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://de.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://kd.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ur.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ry.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://zk.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yp.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xo.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xm.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tt.huanxung.cn

Go:   func add(a, b int) int
来源：http://zy.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lp.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pn.panjiajie.cn

[C14] 泛型函数
来源：http://pl.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iz.yuexingan06.cn

PHP:  // 无泛型
来源：http://zg.9csxet.cn

JS:   // 无泛型
来源：http://ej.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hk.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pu.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ki.newstarts.cn

Ruby: # 无泛型
来源：http://fj.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kd.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://hx.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iz.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://bx.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ve.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fq.chemitech.net.cn

Java: // 无解构
来源：http://lu.lnxyls.cn

Go:   // 无解构
来源：http://ba.hnjuh.cn

Ruby: a, b = pair
来源：http://ic.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://sq.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://rg.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lp.szsharing.cn

PHP:  // 无重载
来源：http://bm.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cz.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://fb.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oa.521024.cn

Go:   // 无重载：用不同函数名
来源：http://zq.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://le.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rn.lnxyls.cn

================================================================================
来源：http://tn.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ha.colortex.cn

================================================================================
来源：http://vj.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://qr.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ec.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://np.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rg.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fy.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rz.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ns.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://ma.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fs.asd995.cn

[D02] 追加元素到末尾
来源：http://jl.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wy.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qv.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://lp.lnxyls.cn

TS:   arr.push(4);
来源：http://gx.huixinmuqiang.cn

Java: list.add(4);
来源：http://yu.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://lu.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://pt.yuexingan06.cn

C#:   list.Add(4);
来源：http://td.nszjky.cn

[D03] 在指定位置插入元素
来源：http://fd.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://zf.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ho.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ec.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://yf.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://jc.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fy.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ee.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://au.jctech888.com.cn

[D04] 删除元素
来源：http://gw.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wv.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://go.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rz.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://mw.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pv.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://km.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lf.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rt.muxihuayi.cn

[D05] 访问与修改元素
来源：http://mc.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ef.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kd.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cv.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://kq.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://xp.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://hk.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xt.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qq.muxihuayi.cn

[D06] 数组长度
来源：http://kq.szxytkj.cn

Py:   len(arr)
来源：http://ow.lnxyls.cn

PHP:  count($arr);
来源：http://ds.asd995.cn

JS:   arr.length
来源：http://el.shxzskj.cn

TS:   arr.length
来源：http://tl.asd995.cn

Java: list.size();
来源：http://hg.521024.cn

Go:   len(arr)
来源：http://df.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://ou.huixiangedu.cn

C#:   list.Count;
来源：http://js.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://ht.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bj.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tu.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://vs.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://vq.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://rp.shxzskj.cn

Go:   arr[1:4]
来源：http://qm.nicolike.cn

Ruby: arr[1, 3]
来源：http://ce.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://gs.shxzukj.cn

[D08] 合并两个数组
来源：http://ey.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://rn.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://he.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gq.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://kz.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wi.nszjky.cn

Go:   append(a, b...)
来源：http://jx.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://kx.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://gm.panjiajie.cn

[D09] 排序（升序）
来源：http://rr.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://gb.shxzukj.cn

PHP:  sort($arr);
来源：http://bh.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nd.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ow.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hj.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zf.panjiajie.cn

Ruby: arr.sort
来源：http://pu.jctech888.com.cn

C#:   list.Sort();
来源：http://ne.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zm.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ua.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eq.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xf.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ih.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://df.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dk.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ye.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vd.huanxung.cn

[D11] 反转数组
来源：http://kv.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xj.newstarts.cn

PHP:  array_reverse($arr);
来源：http://tn.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yr.szsharing.cn

TS:   [...arr].reverse();
来源：http://hj.panjiajie.cn

Java: Collections.reverse(list);
来源：http://mm.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ic.newstarts.cn

Ruby: arr.reverse
来源：http://jr.bjjhwx.cn

C#:   list.Reverse();
来源：http://ax.yuexingan06.cn

[D12] 查找元素下标
来源：http://ir.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ut.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nw.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ii.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ti.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wz.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://qv.lnxyls.cn

Ruby: arr.index(x)
来源：http://yg.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://mo.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://ny.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xs.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mv.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://jb.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://hw.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cb.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xf.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dm.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wz.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://qk.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mb.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bj.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://cj.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://si.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ok.521024.cn

Go:   // 手写循环
来源：http://xb.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mj.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lt.shxzskj.cn

[D15] 去重
来源：http://to.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dx.shxzskj.cn

PHP:  array_unique($arr);
来源：http://lz.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://fm.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ig.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ll.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gb.huanxung.cn

Ruby: arr.uniq
来源：http://vd.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://fo.nszjky.cn

[D16] 求和与平均值
来源：http://gx.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oy.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jx.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ci.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dh.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aa.huanxung.cn

Go:   // 手写循环累加
来源：http://rr.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wy.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://hn.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://nc.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://jq.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://jo.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wj.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://xk.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xq.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ad.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://ko.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ac.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xa.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://ee.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dy.bookmarksfly.cn

TS:   nested.flat();
来源：http://ql.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fx.colortex.cn

Go:   // 手写双层循环
来源：http://ur.bjjhwx.cn

Ruby: nested.flatten
来源：http://za.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kr.wgjwhj.cn

[D19] 按字段分组
来源：http://zf.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gc.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pe.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jh.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hw.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fn.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://dc.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xt.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iz.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://zj.newstarts.cn

Py:   Counter(arr)
来源：http://et.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://au.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iv.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qj.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iz.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://np.hahajie.cn

Ruby: arr.tally
来源：http://ia.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://no.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://cf.asd995.cn

Py:   x in arr
来源：http://dt.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://go.asd995.cn

JS:   arr.includes(x)
来源：http://kz.colortex.cn

TS:   arr.includes(x)
来源：http://si.shxzskj.cn

Java: list.contains(x)
来源：http://aq.jctech888.com.cn


<!-- 参考信息 -->