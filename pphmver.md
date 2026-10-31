代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://zy.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://pz.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zd.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://to.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kc.huixiangedu.cn

TS:   arr.map(String)
来源：http://cl.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://un.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jr.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://fz.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cq.shxzukj.cn

[C08] 闭包
来源：http://iu.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dv.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mj.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cx.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xh.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gj.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nl.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://up.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iy.huixiangedu.cn

[C09] 递归
来源：http://bu.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ta.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cz.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fw.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://du.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ww.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xp.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wq.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://il.shxzukj.cn

[C10] 变量作用域
来源：http://vv.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kg.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://de.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tf.chemitech.net.cn

TS:   同 JS
来源：http://uh.colortex.cn

Java: 方法内为块级作用域
来源：http://ps.hnjuh.cn

Go:   花括号块级作用域
来源：http://md.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ae.panjiajie.cn

C#:   块级作用域
来源：http://oi.yuexingan06.cn

[C11] 模块导入与导出
来源：http://yq.yuntaijiaju.cn

Py:   from module import func
来源：http://xo.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nh.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nr.hnjuh.cn

Java: import java.util.List;
来源：http://ej.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://be.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://oq.colortex.cn

C#:   using System.Text;
来源：http://xo.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://yh.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://cr.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://nh.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://il.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://qg.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ww.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ba.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://gn.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jw.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://bg.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fo.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iz.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fq.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kv.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lr.shxzukj.cn

Go:   func add(a, b int) int
来源：http://gt.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wr.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yh.szsharing.cn

[C14] 泛型函数
来源：http://sv.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jg.521024.cn

PHP:  // 无泛型
来源：http://xs.yuntaijiaju.cn

JS:   // 无泛型
来源：http://bj.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ii.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qr.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ae.panjiajie.cn

Ruby: # 无泛型
来源：http://zh.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ak.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://aj.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://fp.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qx.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oj.panjiajie.cn

Java: // 无解构
来源：http://ac.shxzskj.cn

Go:   // 无解构
来源：http://ka.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://cx.huanxung.cn

C#:   var (a, b) = pair;
来源：http://tm.newstarts.cn

[C16] 函数 / 方法重载
来源：http://dn.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sa.szsharing.cn

PHP:  // 无重载
来源：http://fc.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kl.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://em.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tm.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://zn.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://ro.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tz.bookmarksfly.cn

================================================================================
来源：http://ns.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://bv.9csxet.cn

================================================================================
来源：http://yu.9csxet.cn

[D01] 创建数组 / 列表
来源：http://th.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://da.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iu.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gt.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hg.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qe.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://oq.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://gw.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dx.9csxet.cn

[D02] 追加元素到末尾
来源：http://cg.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tt.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ea.shxzukj.cn

JS:   arr.push(4);
来源：http://dg.szsharing.cn

TS:   arr.push(4);
来源：http://ua.chemitech.net.cn

Java: list.add(4);
来源：http://ir.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://ir.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://yk.panjiajie.cn

C#:   list.Add(4);
来源：http://rc.hahajie.cn

[D03] 在指定位置插入元素
来源：http://st.asd995.cn

Py:   arr.insert(0, 0)
来源：http://ti.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tq.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://up.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://zn.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://ey.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vr.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://be.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://uk.haigaiapp.cn

[D04] 删除元素
来源：http://jh.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jv.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rg.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ie.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://xl.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nu.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://he.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vj.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xv.hnjuh.cn

[D05] 访问与修改元素
来源：http://ix.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rk.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://am.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fn.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://ts.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://yw.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://yu.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sa.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cy.chemitech.net.cn

[D06] 数组长度
来源：http://hr.yuexingan06.cn

Py:   len(arr)
来源：http://aw.jctech888.com.cn

PHP:  count($arr);
来源：http://gt.shxzukj.cn

JS:   arr.length
来源：http://mn.wgjwhj.cn

TS:   arr.length
来源：http://wm.asd995.cn

Java: list.size();
来源：http://ld.bjjhwx.cn

Go:   len(arr)
来源：http://pg.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://sq.521024.cn

C#:   list.Count;
来源：http://zy.asd995.cn

[D07] 切片 / 取子数组
来源：http://ps.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fq.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ot.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://xo.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://av.nszjky.cn

Java: list.subList(1, 4);
来源：http://xo.gzmigu.cn

Go:   arr[1:4]
来源：http://rc.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://hi.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://xg.chemitech.net.cn

[D08] 合并两个数组
来源：http://do.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://ve.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://hn.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hk.chemitech.net.cn

TS:   [...a, ...b];
来源：http://xw.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bx.shxzukj.cn

Go:   append(a, b...)
来源：http://pf.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://tu.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://jk.bookmarksfly.cn

[D09] 排序（升序）
来源：http://mq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://vm.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://fh.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mg.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ot.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xy.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fe.panjiajie.cn

Ruby: arr.sort
来源：http://xg.yuexingan06.cn

C#:   list.Sort();
来源：http://du.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lv.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vt.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://db.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aa.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ct.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://au.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mj.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vc.9csxet.cn

[D11] 反转数组
来源：http://vg.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xi.hahajie.cn

PHP:  array_reverse($arr);
来源：http://vw.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://et.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://dy.colortex.cn

Java: Collections.reverse(list);
来源：http://ua.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://vo.huanxung.cn

Ruby: arr.reverse
来源：http://lb.haigaiapp.cn

C#:   list.Reverse();
来源：http://gt.bookmarksfly.cn

[D12] 查找元素下标
来源：http://cq.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://cw.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tw.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rp.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://df.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vs.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://qr.shtwfgs.cn

Ruby: arr.index(x)
来源：http://ue.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://av.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://ik.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ju.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://in.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://zs.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://uy.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qn.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://do.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bd.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lv.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://wx.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mt.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hs.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://mf.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://qp.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oh.shtwfgs.cn

Go:   // 手写循环
来源：http://bg.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qp.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ga.szxytkj.cn

[D15] 去重
来源：http://nb.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pt.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://hu.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://fg.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://dp.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://de.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bu.huanxung.cn

Ruby: arr.uniq
来源：http://sk.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://ja.yuexingan06.cn

[D16] 求和与平均值
来源：http://cq.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jq.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eo.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cr.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rb.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://me.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ft.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xc.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://zq.bjjhwx.cn

[D17] 最大值与最小值
来源：http://bq.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://xp.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://wy.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ht.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://fy.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mj.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://le.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://lx.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://dv.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://gb.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vi.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://ss.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ba.szsharing.cn

TS:   nested.flat();
来源：http://oa.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fm.hahajie.cn

Go:   // 手写双层循环
来源：http://jy.newstarts.cn

Ruby: nested.flatten
来源：http://os.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zi.gzmigu.cn

[D19] 按字段分组
来源：http://cf.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wu.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gd.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rb.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vz.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ke.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://kp.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://od.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ew.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://tk.9csxet.cn

Py:   Counter(arr)
来源：http://kk.hahajie.cn

PHP:  array_count_values($arr);
来源：http://th.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ys.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dj.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kf.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://my.hnjuh.cn

Ruby: arr.tally
来源：http://vi.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mq.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://vc.colortex.cn

Py:   x in arr
来源：http://jl.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://hx.chemitech.net.cn

JS:   arr.includes(x)
来源：http://di.shxzskj.cn

TS:   arr.includes(x)
来源：http://zk.nicolike.cn

Java: list.contains(x)
来源：http://pe.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://cn.gzmigu.cn

Ruby: arr.include?(x)
来源：http://qg.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://he.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://rz.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cw.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qi.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nj.shxzskj.cn

TS:   [...arr];
来源：http://mx.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://pz.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cy.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://ju.newstarts.cn

C#:   new List<int>(list);
来源：http://xz.lnxyls.cn

[D23] reduce 累积计算
来源：http://xh.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://er.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ls.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jm.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rq.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fh.gzmigu.cn

Go:   // 手写循环
来源：http://hk.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iw.yuntaijiaju.cn


<!-- 参考信息 -->