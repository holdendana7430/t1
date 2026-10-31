代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tp.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iw.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iy.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ht.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://mt.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://ga.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://nh.newstarts.cn

[C05] 返回多个值
来源：http://vx.bjjhwx.cn

Py:   return a, b
来源：http://xj.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://vh.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pz.bookmarksfly.cn

TS:   return { a, b };
来源：http://wx.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gy.shxzukj.cn

Go:   return a, b
来源：http://mt.muxihuayi.cn

Ruby: return a, b
来源：http://qi.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://rw.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://wd.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://yv.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vw.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://xn.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://sm.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://et.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://td.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://xw.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ni.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://sz.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://re.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kr.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ao.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://nn.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zd.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kr.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://jn.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pz.huixinmuqiang.cn

[C08] 闭包
来源：http://rr.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fu.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ih.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hf.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ex.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ee.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zz.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qe.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ss.shxzukj.cn

[C09] 递归
来源：http://be.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://py.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://do.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jm.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sb.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://la.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://if.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ko.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://in.haigaiapp.cn

[C10] 变量作用域
来源：http://dp.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://to.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pe.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xk.hnjuh.cn

TS:   同 JS
来源：http://lq.huanxung.cn

Java: 方法内为块级作用域
来源：http://pj.muxihuayi.cn

Go:   花括号块级作用域
来源：http://bh.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mj.9csxet.cn

C#:   块级作用域
来源：http://gb.szxytkj.cn

[C11] 模块导入与导出
来源：http://de.huanxung.cn

Py:   from module import func
来源：http://cr.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hg.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ik.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lv.chemitech.net.cn

Java: import java.util.List;
来源：http://xs.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bx.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ly.muxihuayi.cn

C#:   using System.Text;
来源：http://wd.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://gl.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://vo.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://ti.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://mx.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://um.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sw.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://ro.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://yg.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cu.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://ap.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://if.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zf.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bj.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ab.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://la.gzmigu.cn

Go:   func add(a, b int) int
来源：http://pi.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sm.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gh.shxzukj.cn

[C14] 泛型函数
来源：http://wh.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zh.gzmigu.cn

PHP:  // 无泛型
来源：http://jh.shxzskj.cn

JS:   // 无泛型
来源：http://uz.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://go.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fg.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qh.shxzukj.cn

Ruby: # 无泛型
来源：http://sh.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ig.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://av.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bk.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://cm.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vj.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://go.shxzukj.cn

Java: // 无解构
来源：http://yl.haigaiapp.cn

Go:   // 无解构
来源：http://qb.wgjwhj.cn

Ruby: a, b = pair
来源：http://nl.9csxet.cn

C#:   var (a, b) = pair;
来源：http://ck.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://tw.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nu.lnxyls.cn

PHP:  // 无重载
来源：http://yk.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vv.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://qg.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sy.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://zh.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://kq.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xi.haigaiapp.cn

================================================================================
来源：http://rp.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://kp.newstarts.cn

================================================================================
来源：http://uh.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://qj.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jj.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oe.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mj.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://te.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nt.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ld.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://to.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vy.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://mg.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://an.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fn.shtwfgs.cn

JS:   arr.push(4);
来源：http://ly.colortex.cn

TS:   arr.push(4);
来源：http://dm.hahajie.cn

Java: list.add(4);
来源：http://re.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://hv.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://nd.bjjhwx.cn

C#:   list.Add(4);
来源：http://ei.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://pw.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://lb.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ev.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zu.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://ts.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://np.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eo.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tf.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://tm.bookmarksfly.cn

[D04] 删除元素
来源：http://px.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ar.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yo.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://au.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://fm.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dr.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wg.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pd.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hs.bjjhwx.cn

[D05] 访问与修改元素
来源：http://fc.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fg.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://td.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hr.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://gk.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://wm.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://zm.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xs.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bc.colortex.cn

[D06] 数组长度
来源：http://ur.huanxung.cn

Py:   len(arr)
来源：http://rn.hahajie.cn

PHP:  count($arr);
来源：http://zj.wgjwhj.cn

JS:   arr.length
来源：http://bo.nicolike.cn

TS:   arr.length
来源：http://ez.panjiajie.cn

Java: list.size();
来源：http://op.newstarts.cn

Go:   len(arr)
来源：http://bo.nicolike.cn

Ruby: arr.length; arr.size
来源：http://ls.huixinmuqiang.cn

C#:   list.Count;
来源：http://mi.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://by.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ny.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://un.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://nq.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://yr.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://it.nszjky.cn

Go:   arr[1:4]
来源：http://vw.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://ai.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://jy.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://hp.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://uk.asd995.cn

PHP:  array_merge($a, $b);
来源：http://vz.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ey.chemitech.net.cn

TS:   [...a, ...b];
来源：http://qm.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ie.shxzskj.cn

Go:   append(a, b...)
来源：http://ms.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://wn.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://jo.szsharing.cn

[D09] 排序（升序）
来源：http://sh.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://uh.lnxyls.cn

PHP:  sort($arr);
来源：http://ww.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wb.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fu.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uh.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pv.hahajie.cn

Ruby: arr.sort
来源：http://cf.bjjhwx.cn

C#:   list.Sort();
来源：http://lt.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fr.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://do.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://np.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://db.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ob.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tt.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rk.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ui.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jh.chemitech.net.cn

[D11] 反转数组
来源：http://aw.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://za.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ye.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fm.newstarts.cn

TS:   [...arr].reverse();
来源：http://un.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://ex.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ak.hnjuh.cn

Ruby: arr.reverse
来源：http://jb.hnjuh.cn

C#:   list.Reverse();
来源：http://md.shxzukj.cn

[D12] 查找元素下标
来源：http://tf.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://re.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sc.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dd.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tx.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sd.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://ic.hnjuh.cn

Ruby: arr.index(x)
来源：http://ik.newstarts.cn

C#:   list.IndexOf(x);
来源：http://bh.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://mr.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sx.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xy.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://mx.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ij.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://th.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pe.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cp.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yh.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://kw.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kp.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kh.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://am.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://km.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yn.shxzukj.cn

Go:   // 手写循环
来源：http://ee.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vr.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kh.wgjwhj.cn

[D15] 去重
来源：http://ys.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ju.hahajie.cn

PHP:  array_unique($arr);
来源：http://tw.nszjky.cn

JS:   [...new Set(arr)]
来源：http://on.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://te.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ix.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wd.panjiajie.cn

Ruby: arr.uniq
来源：http://xn.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://sx.shtwfgs.cn

[D16] 求和与平均值
来源：http://qg.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wh.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ut.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yy.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lf.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ot.yuexingan06.cn

Go:   // 手写循环累加
来源：http://qg.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://an.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ue.hnjuh.cn

[D17] 最大值与最小值
来源：http://vo.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ni.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://cx.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zl.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://ja.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://se.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cg.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://tq.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://gd.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://mt.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ts.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://cr.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dq.chemitech.net.cn

TS:   nested.flat();
来源：http://hd.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://td.lnxyls.cn

Go:   // 手写双层循环
来源：http://bf.bjjhwx.cn

Ruby: nested.flatten
来源：http://un.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://es.jianghongdianzi.cn

[D19] 按字段分组
来源：http://no.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qn.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aw.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://su.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zh.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oe.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://al.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rm.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dt.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://zs.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://bd.szsharing.cn

PHP:  array_count_values($arr);
来源：http://qw.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ro.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xa.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://np.nicolike.cn

Go:   // 手写 map[T]int
来源：http://fq.nicolike.cn

Ruby: arr.tally
来源：http://gg.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ih.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://st.jianghongdianzi.cn

Py:   x in arr
来源：http://cr.shtwfgs.cn


<!-- 参考信息 -->