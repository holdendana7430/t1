代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hf.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://pr.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://gn.shxzukj.cn

[C05] 返回多个值
来源：http://qo.jianghongdianzi.cn

Py:   return a, b
来源：http://ku.asd995.cn

PHP:  return [$a, $b];
来源：http://wn.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ol.nicolike.cn

TS:   return { a, b };
来源：http://eb.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tg.hnjuh.cn

Go:   return a, b
来源：http://jc.yuexingan06.cn

Ruby: return a, b
来源：http://cs.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://sq.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://tg.nszjky.cn

Py:   square = lambda x: x * x
来源：http://fd.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ac.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://yj.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://je.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ct.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zf.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://er.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kx.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://zv.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bf.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://px.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qp.jctech888.com.cn

TS:   arr.map(String)
来源：http://po.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ly.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ix.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://za.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sn.521024.cn

[C08] 闭包
来源：http://bf.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://py.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qo.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gs.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vw.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cq.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yn.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rl.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ot.newstarts.cn

[C09] 递归
来源：http://qy.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sf.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ck.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wa.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vb.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://py.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tv.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qa.colortex.cn

[C10] 变量作用域
来源：http://vm.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fi.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ci.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yn.panjiajie.cn

TS:   同 JS
来源：http://gl.lnxyls.cn

Java: 方法内为块级作用域
来源：http://db.panjiajie.cn

Go:   花括号块级作用域
来源：http://eo.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lv.521024.cn

C#:   块级作用域
来源：http://iv.muxihuayi.cn

[C11] 模块导入与导出
来源：http://xt.asd995.cn

Py:   from module import func
来源：http://rf.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xu.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bc.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eq.asd995.cn

Java: import java.util.List;
来源：http://ai.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eh.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://cv.muxihuayi.cn

C#:   using System.Text;
来源：http://cv.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://nu.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ux.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://xh.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ii.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://lk.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://av.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://ln.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://wc.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yw.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://rk.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bm.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://or.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fw.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://je.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://ob.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fh.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gc.lnxyls.cn

[C14] 泛型函数
来源：http://nh.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hw.hnjuh.cn

PHP:  // 无泛型
来源：http://nv.szsharing.cn

JS:   // 无泛型
来源：http://pj.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ru.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ze.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vk.9csxet.cn

Ruby: # 无泛型
来源：http://pw.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hr.szsharing.cn

[C15] 解构 / 展开参数
来源：http://gi.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ka.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://qi.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xo.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iy.szxytkj.cn

Java: // 无解构
来源：http://cz.nszjky.cn

Go:   // 无解构
来源：http://eo.panjiajie.cn

Ruby: a, b = pair
来源：http://ca.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://od.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://nb.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://am.hnjuh.cn

PHP:  // 无重载
来源：http://qe.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nc.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://lm.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qk.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ad.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://pe.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ro.hnjuh.cn

================================================================================
来源：http://pp.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://vg.nicolike.cn

[D01] 创建数组 / 列表
来源：http://ta.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://od.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fq.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yc.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mz.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ss.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://hv.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://td.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ih.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ev.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kc.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gz.panjiajie.cn

JS:   arr.push(4);
来源：http://zs.haigaiapp.cn

TS:   arr.push(4);
来源：http://la.szsharing.cn

Java: list.add(4);
来源：http://uo.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://gn.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vk.chemitech.net.cn

C#:   list.Add(4);
来源：http://uf.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ff.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://uy.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yc.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bd.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://pv.yuexingan06.cn

Java: list.add(0, 0);
来源：http://at.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ib.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://it.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://dv.newstarts.cn

[D04] 删除元素
来源：http://tt.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://co.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bo.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oo.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://la.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wi.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cs.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zl.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hd.521024.cn

[D05] 访问与修改元素
来源：http://cu.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ah.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nu.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ks.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://an.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://dn.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://hv.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dg.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://is.newstarts.cn

[D06] 数组长度
来源：http://hz.521024.cn

Py:   len(arr)
来源：http://vv.haigaiapp.cn

PHP:  count($arr);
来源：http://jq.9csxet.cn

JS:   arr.length
来源：http://ms.szsharing.cn

TS:   arr.length
来源：http://aw.gzmigu.cn

Java: list.size();
来源：http://as.shtwfgs.cn

Go:   len(arr)
来源：http://bt.colortex.cn

Ruby: arr.length; arr.size
来源：http://kp.hnjuh.cn

C#:   list.Count;
来源：http://ol.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://yk.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zq.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kc.521024.cn

JS:   arr.slice(1, 4);
来源：http://lv.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://yl.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://xv.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://ao.lnxyls.cn

Ruby: arr[1, 3]
来源：http://us.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://ik.huanxung.cn

[D08] 合并两个数组
来源：http://xh.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://jm.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://cr.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hr.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://wi.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ia.szsharing.cn

Go:   append(a, b...)
来源：http://lx.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://jv.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ne.panjiajie.cn

[D09] 排序（升序）
来源：http://pn.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://oq.521024.cn

PHP:  sort($arr);
来源：http://xo.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gl.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xp.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gi.newstarts.cn

Ruby: arr.sort
来源：http://gw.hahajie.cn

C#:   list.Sort();
来源：http://yz.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rj.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://es.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vz.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kk.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ob.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ke.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ea.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ia.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://du.jianghongdianzi.cn

[D11] 反转数组
来源：http://ul.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vu.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://an.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qh.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://uc.lnxyls.cn

Java: Collections.reverse(list);
来源：http://pd.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://vu.jctech888.com.cn

Ruby: arr.reverse
来源：http://ka.szxytkj.cn

C#:   list.Reverse();
来源：http://ss.jctech888.com.cn

[D12] 查找元素下标
来源：http://mj.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://tl.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cf.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jk.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://me.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rf.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://yv.shxzskj.cn

Ruby: arr.index(x)
来源：http://dn.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://lv.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://zo.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xi.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yn.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://zf.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://vk.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xk.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nu.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qg.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sq.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://da.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rj.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://se.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://xb.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://jp.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://um.shtwfgs.cn

Go:   // 手写循环
来源：http://vg.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wn.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ft.jctech888.com.cn

[D15] 去重
来源：http://td.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lc.panjiajie.cn

PHP:  array_unique($arr);
来源：http://dy.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://ia.hahajie.cn

TS:   [...new Set(arr)]
来源：http://hv.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qs.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ll.bjjhwx.cn

Ruby: arr.uniq
来源：http://gn.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://pa.nszjky.cn

[D16] 求和与平均值
来源：http://mh.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dc.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://es.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rj.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zx.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sa.521024.cn

Go:   // 手写循环累加
来源：http://kg.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://la.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://jq.newstarts.cn

[D17] 最大值与最小值
来源：http://xx.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://kj.521024.cn

PHP:  max($arr);  min($arr);
来源：http://gz.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fs.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://mg.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://at.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mx.521024.cn

Ruby: arr.max;  arr.min
来源：http://xf.521024.cn

C#:   list.Max();  list.Min()
来源：http://eg.asd995.cn

[D18] 扁平化嵌套数组
来源：http://jv.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sq.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://kx.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dh.wgjwhj.cn

TS:   nested.flat();
来源：http://wq.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ui.colortex.cn

Go:   // 手写双层循环
来源：http://oo.lnxyls.cn

Ruby: nested.flatten
来源：http://yc.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xw.huanxung.cn

[D19] 按字段分组
来源：http://za.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://df.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dk.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xk.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fv.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://za.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://ua.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cv.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sc.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://iu.szxytkj.cn

Py:   Counter(arr)
来源：http://hz.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://ch.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lw.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ds.colortex.cn

Go:   // 手写 map[T]int
来源：http://ku.yuexingan06.cn

Ruby: arr.tally
来源：http://cp.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zy.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://eb.huixinmuqiang.cn

Py:   x in arr
来源：http://wf.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://pf.shxzskj.cn

JS:   arr.includes(x)
来源：http://ug.yuexingan06.cn

TS:   arr.includes(x)
来源：http://hy.haigaiapp.cn

Java: list.contains(x)
来源：http://mg.gzmigu.cn


<!-- 参考信息 -->