代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ss.jctech888.com.cn

Go:   return a, b
来源：http://an.huixinmuqiang.cn

Ruby: return a, b
来源：http://bu.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://sz.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://qm.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://em.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xq.hnjuh.cn

JS:   const square = x => x * x;
来源：http://gn.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://xf.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nh.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ds.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ey.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pv.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://sq.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ps.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fe.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lr.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://ch.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rs.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://as.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://cg.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kh.9csxet.cn

[C08] 闭包
来源：http://nt.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kd.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://be.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xb.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jv.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ei.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nx.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://as.yuntaijiaju.cn

[C09] 递归
来源：http://ku.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eg.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lr.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fn.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jw.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://do.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://om.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rg.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ma.shtwfgs.cn

[C10] 变量作用域
来源：http://ot.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ih.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cv.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eo.hahajie.cn

TS:   同 JS
来源：http://xo.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://ht.521024.cn

Go:   花括号块级作用域
来源：http://ov.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mz.huixinmuqiang.cn

C#:   块级作用域
来源：http://uh.521024.cn

[C11] 模块导入与导出
来源：http://hm.9csxet.cn

Py:   from module import func
来源：http://az.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lw.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ni.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fh.huixiangedu.cn

Java: import java.util.List;
来源：http://aj.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ij.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://fe.panjiajie.cn

C#:   using System.Text;
来源：http://nv.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://jg.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://ti.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://cj.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://eg.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://ea.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yq.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://yo.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://vr.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fq.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://qw.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://em.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://um.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ui.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tw.hnjuh.cn

Go:   func add(a, b int) int
来源：http://cl.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dk.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ik.gzmigu.cn

[C14] 泛型函数
来源：http://xx.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rz.shxzukj.cn

PHP:  // 无泛型
来源：http://mo.hnjuh.cn

JS:   // 无泛型
来源：http://zu.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vp.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xg.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zc.szsharing.cn

Ruby: # 无泛型
来源：http://fm.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mo.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://uf.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cj.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://oq.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xw.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lg.wgjwhj.cn

Java: // 无解构
来源：http://dg.wgjwhj.cn

Go:   // 无解构
来源：http://wb.9csxet.cn

Ruby: a, b = pair
来源：http://dh.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://pr.colortex.cn

[C16] 函数 / 方法重载
来源：http://hu.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ty.muxihuayi.cn

PHP:  // 无重载
来源：http://jp.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hk.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://yf.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fa.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://lq.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://fg.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://os.asd995.cn

================================================================================
来源：http://ld.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://lx.nszjky.cn

================================================================================
来源：http://jv.asd995.cn

[D01] 创建数组 / 列表
来源：http://qn.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kn.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fc.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://up.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ek.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gc.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://za.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://jv.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gn.shxzskj.cn

[D02] 追加元素到末尾
来源：http://pd.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xy.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ly.shxzskj.cn

JS:   arr.push(4);
来源：http://li.newstarts.cn

TS:   arr.push(4);
来源：http://oo.yuexingan06.cn

Java: list.add(4);
来源：http://jh.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://vf.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://db.szxytkj.cn

C#:   list.Add(4);
来源：http://en.szsharing.cn

[D03] 在指定位置插入元素
来源：http://hk.asd995.cn

Py:   arr.insert(0, 0)
来源：http://ij.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wa.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eo.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://hy.chemitech.net.cn

Java: list.add(0, 0);
来源：http://mx.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yz.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://js.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://oa.newstarts.cn

[D04] 删除元素
来源：http://fk.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ig.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pz.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lp.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://zd.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bz.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oq.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mu.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ff.hnjuh.cn

[D05] 访问与修改元素
来源：http://jh.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ih.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ri.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sd.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gm.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://pf.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://mc.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://at.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nm.shtwfgs.cn

[D06] 数组长度
来源：http://bt.asd995.cn

Py:   len(arr)
来源：http://of.hahajie.cn

PHP:  count($arr);
来源：http://hq.colortex.cn

JS:   arr.length
来源：http://nh.wgjwhj.cn

TS:   arr.length
来源：http://ch.colortex.cn

Java: list.size();
来源：http://gi.shxzskj.cn

Go:   len(arr)
来源：http://kx.colortex.cn

Ruby: arr.length; arr.size
来源：http://bx.yuexingan06.cn

C#:   list.Count;
来源：http://wa.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://bt.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xt.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gv.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://yc.colortex.cn

TS:   arr.slice(1, 4);
来源：http://oy.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://tm.521024.cn

Go:   arr[1:4]
来源：http://uh.521024.cn

Ruby: arr[1, 3]
来源：http://wm.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://pc.bjjhwx.cn

[D08] 合并两个数组
来源：http://yl.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://bx.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://va.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fg.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ji.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pm.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://jy.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://bf.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://ab.yuexingan06.cn

[D09] 排序（升序）
来源：http://oa.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fb.muxihuayi.cn

PHP:  sort($arr);
来源：http://vo.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rt.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ta.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gp.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tf.haigaiapp.cn

Ruby: arr.sort
来源：http://je.bookmarksfly.cn

C#:   list.Sort();
来源：http://ls.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zb.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hq.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hd.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iq.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jn.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ky.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cy.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xg.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ke.yuntaijiaju.cn

[D11] 反转数组
来源：http://ms.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mx.asd995.cn

PHP:  array_reverse($arr);
来源：http://ul.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sc.nicolike.cn

TS:   [...arr].reverse();
来源：http://md.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://xk.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://cz.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://nh.gzmigu.cn

C#:   list.Reverse();
来源：http://fx.szxytkj.cn

[D12] 查找元素下标
来源：http://im.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://zu.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cm.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://si.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tb.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ey.asd995.cn

Go:   slices.Index(arr, x)
来源：http://vq.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://kb.9csxet.cn

C#:   list.IndexOf(x);
来源：http://xc.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ck.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ga.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gf.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://my.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://cx.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bv.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dp.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xa.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eo.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://ls.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jq.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gl.521024.cn

JS:   arr.map(x => x * 2)
来源：http://lt.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://nj.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ho.asd995.cn

Go:   // 手写循环
来源：http://aa.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kg.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xl.shxzskj.cn

[D15] 去重
来源：http://ab.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yk.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://iz.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://ef.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://bq.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://be.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kx.szxytkj.cn

Ruby: arr.uniq
来源：http://ti.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://bv.521024.cn

[D16] 求和与平均值
来源：http://lp.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nx.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kr.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ee.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bl.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://om.hnjuh.cn

Go:   // 手写循环累加
来源：http://gb.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ni.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://xv.szxytkj.cn

[D17] 最大值与最小值
来源：http://cx.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://gr.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://at.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://do.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://tm.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eq.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fn.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://vr.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://nd.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://wc.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vr.colortex.cn

PHP:  array_merge(...$nested);
来源：http://zt.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qs.hnjuh.cn

TS:   nested.flat();
来源：http://jg.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yd.asd995.cn

Go:   // 手写双层循环
来源：http://vv.szxytkj.cn

Ruby: nested.flatten
来源：http://qn.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zu.colortex.cn

[D19] 按字段分组
来源：http://sv.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ni.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ur.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vh.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bk.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ua.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://dd.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sv.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dk.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://du.hahajie.cn

Py:   Counter(arr)
来源：http://zu.9csxet.cn

PHP:  array_count_values($arr);
来源：http://yx.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zy.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ay.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ar.9csxet.cn

Go:   // 手写 map[T]int
来源：http://xc.9csxet.cn

Ruby: arr.tally
来源：http://ty.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ro.nicolike.cn

[D21] 判断是否包含某元素
来源：http://yc.nszjky.cn

Py:   x in arr
来源：http://zy.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://fb.bjjhwx.cn

JS:   arr.includes(x)
来源：http://bb.haigaiapp.cn

TS:   arr.includes(x)
来源：http://el.huanxung.cn

Java: list.contains(x)
来源：http://lx.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://id.szsharing.cn

Ruby: arr.include?(x)
来源：http://cj.panjiajie.cn

C#:   list.Contains(x)
来源：http://gz.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://oe.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gw.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qk.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bg.asd995.cn

TS:   [...arr];
来源：http://nm.muxihuayi.cn


<!-- 参考信息 -->