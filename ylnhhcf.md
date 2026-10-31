代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ku.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://kc.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wo.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oa.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hi.jctech888.com.cn

TS:   arr.map(String)
来源：http://js.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://es.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pl.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://hk.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vr.shxzukj.cn

[C08] 闭包
来源：http://no.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ow.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://je.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lt.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kv.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vb.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sm.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ix.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ds.bjjhwx.cn

[C09] 递归
来源：http://te.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://so.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://os.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vp.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xu.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rx.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eo.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xl.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iq.yuexingan06.cn

[C10] 变量作用域
来源：http://qo.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ho.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://on.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://la.shxzskj.cn

TS:   同 JS
来源：http://ao.szxytkj.cn

Java: 方法内为块级作用域
来源：http://be.lnxyls.cn

Go:   花括号块级作用域
来源：http://vc.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xx.szsharing.cn

C#:   块级作用域
来源：http://xc.huixiangedu.cn

[C11] 模块导入与导出
来源：http://lq.newstarts.cn

Py:   from module import func
来源：http://gl.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zr.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gj.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fk.bookmarksfly.cn

Java: import java.util.List;
来源：http://yv.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aq.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://cd.szxytkj.cn

C#:   using System.Text;
来源：http://oo.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://xz.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://sh.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://lf.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://te.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://vf.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tg.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://vo.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://fx.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sh.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://eg.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cp.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qx.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ly.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gt.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dk.9csxet.cn

Go:   func add(a, b int) int
来源：http://uz.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cd.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wu.gzmigu.cn

[C14] 泛型函数
来源：http://du.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zq.szxytkj.cn

PHP:  // 无泛型
来源：http://op.wgjwhj.cn

JS:   // 无泛型
来源：http://tc.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fk.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gn.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ax.jctech888.com.cn

Ruby: # 无泛型
来源：http://dm.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sp.hahajie.cn

[C15] 解构 / 展开参数
来源：http://yz.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gg.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://ia.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://it.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kz.newstarts.cn

Java: // 无解构
来源：http://jo.9csxet.cn

Go:   // 无解构
来源：http://ke.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://do.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ct.szsharing.cn

[C16] 函数 / 方法重载
来源：http://ix.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ix.yuexingan06.cn

PHP:  // 无重载
来源：http://iu.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nj.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://sb.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pe.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://cy.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://yr.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qm.lnxyls.cn

================================================================================
来源：http://gf.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ln.shtwfgs.cn

================================================================================
来源：http://lu.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://rc.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rf.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wn.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://up.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uk.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gp.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ko.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://zf.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dg.nicolike.cn

[D02] 追加元素到末尾
来源：http://jh.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://be.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nm.bookmarksfly.cn

JS:   arr.push(4);
来源：http://vh.gzmigu.cn

TS:   arr.push(4);
来源：http://ev.huixinmuqiang.cn

Java: list.add(4);
来源：http://yd.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://hl.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ay.9csxet.cn

C#:   list.Add(4);
来源：http://hz.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://xs.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://ff.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pc.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yh.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://jg.jctech888.com.cn

Java: list.add(0, 0);
来源：http://bk.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mk.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wy.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://qv.shxzskj.cn

[D04] 删除元素
来源：http://im.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wt.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vb.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ax.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://np.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oy.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cc.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ts.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ux.huixiangedu.cn

[D05] 访问与修改元素
来源：http://yu.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://la.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oi.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://gc.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://fk.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://zv.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gi.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ys.asd995.cn

[D06] 数组长度
来源：http://fy.huixiangedu.cn

Py:   len(arr)
来源：http://ts.shtwfgs.cn

PHP:  count($arr);
来源：http://ks.nszjky.cn

JS:   arr.length
来源：http://qc.panjiajie.cn

TS:   arr.length
来源：http://tz.521024.cn

Java: list.size();
来源：http://jc.nszjky.cn

Go:   len(arr)
来源：http://xf.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://ms.huanxung.cn

C#:   list.Count;
来源：http://tq.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://qq.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ci.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vy.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://yd.521024.cn

TS:   arr.slice(1, 4);
来源：http://yx.panjiajie.cn

Java: list.subList(1, 4);
来源：http://jk.colortex.cn

Go:   arr[1:4]
来源：http://mq.huanxung.cn

Ruby: arr[1, 3]
来源：http://jv.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://yh.muxihuayi.cn

[D08] 合并两个数组
来源：http://fu.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://uo.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://pn.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zw.shxzskj.cn

TS:   [...a, ...b];
来源：http://ey.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pg.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://cy.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://gp.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://xa.yuexingan06.cn

[D09] 排序（升序）
来源：http://nd.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jh.shxzukj.cn

PHP:  sort($arr);
来源：http://rd.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zr.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bo.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tn.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bg.yuexingan06.cn

Ruby: arr.sort
来源：http://ga.panjiajie.cn

C#:   list.Sort();
来源：http://uw.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://it.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bu.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://td.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zm.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://on.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sy.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qp.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wh.lnxyls.cn

[D11] 反转数组
来源：http://dc.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bj.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://iw.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zi.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://tx.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://zu.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://gz.chemitech.net.cn

Ruby: arr.reverse
来源：http://pw.szsharing.cn

C#:   list.Reverse();
来源：http://ar.shxzskj.cn

[D12] 查找元素下标
来源：http://xo.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://uq.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://av.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wj.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uw.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lx.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://zg.jctech888.com.cn

Ruby: arr.index(x)
来源：http://bo.nszjky.cn

C#:   list.IndexOf(x);
来源：http://ey.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://yk.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tb.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jh.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://lc.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://fr.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wp.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hm.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qu.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ny.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://nq.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dk.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://du.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://yu.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://hm.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kv.muxihuayi.cn

Go:   // 手写循环
来源：http://co.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cl.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zc.gzmigu.cn

[D15] 去重
来源：http://nr.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fp.lnxyls.cn

PHP:  array_unique($arr);
来源：http://cr.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://er.colortex.cn

TS:   [...new Set(arr)]
来源：http://gf.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ge.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oi.chemitech.net.cn

Ruby: arr.uniq
来源：http://nr.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://nt.szsharing.cn

[D16] 求和与平均值
来源：http://wd.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lm.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://du.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bl.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jj.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://go.szsharing.cn

Go:   // 手写循环累加
来源：http://ee.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pr.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://va.shxzukj.cn

[D17] 最大值与最小值
来源：http://hj.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://kv.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://iy.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yq.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://pe.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ph.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://av.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://ew.521024.cn

C#:   list.Max();  list.Min()
来源：http://oj.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://ql.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://js.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://xx.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://um.shtwfgs.cn

TS:   nested.flat();
来源：http://ic.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ke.shtwfgs.cn

Go:   // 手写双层循环
来源：http://zc.wgjwhj.cn

Ruby: nested.flatten
来源：http://my.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bc.lnxyls.cn

[D19] 按字段分组
来源：http://wc.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pa.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sr.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fh.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jg.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uy.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://vi.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://as.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lb.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://tu.bookmarksfly.cn

Py:   Counter(arr)
来源：http://hr.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://mt.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://go.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mp.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rp.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://js.nszjky.cn

Ruby: arr.tally
来源：http://wd.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nf.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://nx.huanxung.cn

Py:   x in arr
来源：http://fb.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://vi.nszjky.cn

JS:   arr.includes(x)
来源：http://vm.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://uz.shxzukj.cn

Java: list.contains(x)
来源：http://ir.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://fe.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://rh.asd995.cn

C#:   list.Contains(x)
来源：http://gn.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://wv.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lz.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ko.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zj.nicolike.cn

TS:   [...arr];
来源：http://wg.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://cc.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zp.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://kw.haigaiapp.cn

C#:   new List<int>(list);
来源：http://nr.nicolike.cn

[D23] reduce 累积计算
来源：http://pg.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ks.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zz.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ey.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://og.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bb.521024.cn

Go:   // 手写循环
来源：http://po.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vm.huixinmuqiang.cn


<!-- 参考信息 -->