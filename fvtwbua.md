代发 wailian999

Py:   return a, b
来源：http://ae.hahajie.cn

PHP:  return [$a, $b];
来源：http://jy.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kc.bookmarksfly.cn

TS:   return { a, b };
来源：http://yi.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ry.jianghongdianzi.cn

Go:   return a, b
来源：http://ph.huixiangedu.cn

Ruby: return a, b
来源：http://ty.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://au.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://nx.hahajie.cn

Py:   square = lambda x: x * x
来源：http://wj.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://da.panjiajie.cn

JS:   const square = x => x * x;
来源：http://il.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://pn.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qc.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hl.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ea.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sj.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://bt.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://as.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ij.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://af.haigaiapp.cn

TS:   arr.map(String)
来源：http://wb.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qp.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nm.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://rp.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xj.gzmigu.cn

[C08] 闭包
来源：http://ij.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uo.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ch.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zg.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ot.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vd.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mb.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ka.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ya.huixiangedu.cn

[C09] 递归
来源：http://cy.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uz.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sx.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cv.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fk.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rh.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://og.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pn.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sc.521024.cn

[C10] 变量作用域
来源：http://ae.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wd.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iu.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ur.huanxung.cn

TS:   同 JS
来源：http://em.szsharing.cn

Java: 方法内为块级作用域
来源：http://pr.muxihuayi.cn

Go:   花括号块级作用域
来源：http://bt.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hr.hahajie.cn

C#:   块级作用域
来源：http://hz.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ad.jianghongdianzi.cn

Py:   from module import func
来源：http://dl.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://by.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zx.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pu.haigaiapp.cn

Java: import java.util.List;
来源：http://za.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ki.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://rz.jctech888.com.cn

C#:   using System.Text;
来源：http://db.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://gn.asd995.cn

Py:   (lambda: print("run"))()
来源：http://uc.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://rk.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ix.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://qm.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wt.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://su.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://pz.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ry.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://zj.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yz.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cx.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kr.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ta.nszjky.cn

Go:   func add(a, b int) int
来源：http://hq.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ka.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mt.nicolike.cn

[C14] 泛型函数
来源：http://ft.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hh.shxzukj.cn

PHP:  // 无泛型
来源：http://zd.yuexingan06.cn

JS:   // 无泛型
来源：http://bk.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gt.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yt.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lc.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://ih.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lc.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ia.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://na.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://il.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yb.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ed.gzmigu.cn

Java: // 无解构
来源：http://ck.nicolike.cn

Go:   // 无解构
来源：http://ef.lnxyls.cn

Ruby: a, b = pair
来源：http://hw.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ub.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://yn.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tw.jianghongdianzi.cn

PHP:  // 无重载
来源：http://na.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://he.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://di.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://wc.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://cz.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wl.yuntaijiaju.cn

================================================================================
来源：http://rl.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://oo.521024.cn

================================================================================
来源：http://ir.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://tf.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ve.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hn.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nm.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wa.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ky.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://vm.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://at.nicolike.cn

[D02] 追加元素到末尾
来源：http://jp.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xx.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tq.chemitech.net.cn

JS:   arr.push(4);
来源：http://ff.bjjhwx.cn

TS:   arr.push(4);
来源：http://fp.9csxet.cn

Java: list.add(4);
来源：http://gj.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ph.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://yz.lnxyls.cn

C#:   list.Add(4);
来源：http://lk.9csxet.cn

[D03] 在指定位置插入元素
来源：http://ho.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://vi.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fd.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fr.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://bc.szsharing.cn

Java: list.add(0, 0);
来源：http://tp.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lm.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ur.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://eo.9csxet.cn

[D04] 删除元素
来源：http://tn.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ah.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://us.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rz.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://fk.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fg.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sc.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mb.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rx.huanxung.cn

[D05] 访问与修改元素
来源：http://dk.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cq.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bx.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kx.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://tn.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://um.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ku.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pz.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hs.jianghongdianzi.cn

[D06] 数组长度
来源：http://ju.hnjuh.cn

Py:   len(arr)
来源：http://en.gzmigu.cn

PHP:  count($arr);
来源：http://jd.huixinmuqiang.cn

JS:   arr.length
来源：http://yt.wgjwhj.cn

TS:   arr.length
来源：http://ff.shxzskj.cn

Java: list.size();
来源：http://ai.szsharing.cn

Go:   len(arr)
来源：http://il.asd995.cn

Ruby: arr.length; arr.size
来源：http://oi.haigaiapp.cn

C#:   list.Count;
来源：http://cp.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://bx.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ye.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jy.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://mw.521024.cn

TS:   arr.slice(1, 4);
来源：http://mw.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://dk.bjjhwx.cn

Go:   arr[1:4]
来源：http://td.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://az.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://aj.bjjhwx.cn

[D08] 合并两个数组
来源：http://an.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://rj.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://tu.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://by.gzmigu.cn

TS:   [...a, ...b];
来源：http://xg.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vd.chemitech.net.cn

Go:   append(a, b...)
来源：http://cm.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://xm.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://po.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://ts.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ph.wgjwhj.cn

PHP:  sort($arr);
来源：http://rh.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mi.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ln.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ni.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cz.bookmarksfly.cn

Ruby: arr.sort
来源：http://lo.yuexingan06.cn

C#:   list.Sort();
来源：http://zk.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nv.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yr.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qs.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hd.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ta.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://si.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://re.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://on.szsharing.cn

[D11] 反转数组
来源：http://af.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bb.hahajie.cn

PHP:  array_reverse($arr);
来源：http://dd.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fh.shxzskj.cn

TS:   [...arr].reverse();
来源：http://xm.gzmigu.cn

Java: Collections.reverse(list);
来源：http://fo.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ru.muxihuayi.cn

Ruby: arr.reverse
来源：http://jy.newstarts.cn

C#:   list.Reverse();
来源：http://lf.bookmarksfly.cn

[D12] 查找元素下标
来源：http://kh.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://bp.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gj.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wh.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sp.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ui.muxihuayi.cn

Ruby: arr.index(x)
来源：http://yx.newstarts.cn

C#:   list.IndexOf(x);
来源：http://mu.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://aq.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fm.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pb.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://ou.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://oj.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zz.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nj.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sn.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yq.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://oy.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wl.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yy.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://lp.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://vj.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dk.yuntaijiaju.cn

Go:   // 手写循环
来源：http://nm.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zi.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zq.hahajie.cn

[D15] 去重
来源：http://ok.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xp.gzmigu.cn

PHP:  array_unique($arr);
来源：http://zq.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://jo.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://wv.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rf.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rk.szsharing.cn

Ruby: arr.uniq
来源：http://et.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://cq.szsharing.cn

[D16] 求和与平均值
来源：http://jb.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ed.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rr.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bd.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://de.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fp.huanxung.cn

Go:   // 手写循环累加
来源：http://xx.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zr.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://jf.9csxet.cn

[D17] 最大值与最小值
来源：http://yi.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://nd.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ml.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kb.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://vn.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lj.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uk.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://kj.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://iv.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://pb.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mf.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://nb.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nc.huanxung.cn

TS:   nested.flat();
来源：http://zp.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nb.lnxyls.cn

Go:   // 手写双层循环
来源：http://hs.huixiangedu.cn

Ruby: nested.flatten
来源：http://gp.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bq.hnjuh.cn

[D19] 按字段分组
来源：http://lh.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rx.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wl.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://md.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sn.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cu.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://za.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wl.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://er.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://vo.yuexingan06.cn

Py:   Counter(arr)
来源：http://op.nszjky.cn

PHP:  array_count_values($arr);
来源：http://av.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rn.newstarts.cn

Go:   // 手写 map[T]int
来源：http://db.muxihuayi.cn

Ruby: arr.tally
来源：http://gz.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dm.colortex.cn

[D21] 判断是否包含某元素
来源：http://lm.huixiangedu.cn

Py:   x in arr
来源：http://hg.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://ra.bjjhwx.cn

JS:   arr.includes(x)
来源：http://dd.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://xm.hnjuh.cn

Java: list.contains(x)
来源：http://bp.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://xa.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://sf.colortex.cn

C#:   list.Contains(x)
来源：http://gt.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://ov.shxzskj.cn


<!-- 参考信息 -->