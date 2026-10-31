代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://uh.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://us.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ql.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://yi.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dk.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://vs.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kg.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fv.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zi.hnjuh.cn

TS:   arr.map(String)
来源：http://jz.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rq.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://it.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://ps.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yz.huixinmuqiang.cn

[C08] 闭包
来源：http://uj.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vx.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rl.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jq.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bp.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rr.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oo.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uz.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vz.huanxung.cn

[C09] 递归
来源：http://yq.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://up.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://il.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fl.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wn.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mv.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xq.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bd.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fo.chemitech.net.cn

[C10] 变量作用域
来源：http://oo.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vf.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gk.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ka.521024.cn

TS:   同 JS
来源：http://pd.newstarts.cn

Java: 方法内为块级作用域
来源：http://dv.nicolike.cn

Go:   花括号块级作用域
来源：http://za.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tg.jctech888.com.cn

C#:   块级作用域
来源：http://cu.chemitech.net.cn

[C11] 模块导入与导出
来源：http://tz.szxytkj.cn

Py:   from module import func
来源：http://ko.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mx.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ke.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://st.lnxyls.cn

Java: import java.util.List;
来源：http://mf.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wr.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://su.yuntaijiaju.cn

C#:   using System.Text;
来源：http://hy.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://yv.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://rb.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://ej.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://jb.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://yx.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kt.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://xl.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://iq.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xt.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://ui.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ah.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ts.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://me.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gx.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://me.nszjky.cn

Go:   func add(a, b int) int
来源：http://dr.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nz.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eq.bjjhwx.cn

[C14] 泛型函数
来源：http://oy.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jb.huanxung.cn

PHP:  // 无泛型
来源：http://wr.shxzskj.cn

JS:   // 无泛型
来源：http://fl.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zf.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sj.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qn.huanxung.cn

Ruby: # 无泛型
来源：http://nk.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vd.nszjky.cn

[C15] 解构 / 展开参数
来源：http://fb.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oc.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://le.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qc.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gz.szxytkj.cn

Java: // 无解构
来源：http://qp.jctech888.com.cn

Go:   // 无解构
来源：http://cb.panjiajie.cn

Ruby: a, b = pair
来源：http://xj.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ku.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ld.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rf.shtwfgs.cn

PHP:  // 无重载
来源：http://co.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://er.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://wz.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fl.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://vp.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://vn.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sw.shtwfgs.cn

================================================================================
来源：http://gt.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://sn.chemitech.net.cn

================================================================================
来源：http://hq.nicolike.cn

[D01] 创建数组 / 列表
来源：http://yj.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qc.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gy.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gc.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zl.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mx.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://mz.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bn.szxytkj.cn

[D02] 追加元素到末尾
来源：http://tj.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uy.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ga.yuexingan06.cn

JS:   arr.push(4);
来源：http://rn.hahajie.cn

TS:   arr.push(4);
来源：http://st.yuexingan06.cn

Java: list.add(4);
来源：http://rj.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ym.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://pk.panjiajie.cn

C#:   list.Add(4);
来源：http://sh.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://dn.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://px.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kx.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dn.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://oo.hnjuh.cn

Java: list.add(0, 0);
来源：http://nm.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pd.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fz.asd995.cn

C#:   list.Insert(0, 0);
来源：http://cf.nicolike.cn

[D04] 删除元素
来源：http://ua.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zh.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zc.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kr.521024.cn

TS:   arr.splice(0, 1);
来源：http://pp.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gc.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yk.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gb.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fp.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://xe.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lq.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pa.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dp.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://bp.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://kx.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://qr.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tl.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nq.bookmarksfly.cn

[D06] 数组长度
来源：http://je.huixiangedu.cn

Py:   len(arr)
来源：http://eu.bjjhwx.cn

PHP:  count($arr);
来源：http://jo.shxzskj.cn

JS:   arr.length
来源：http://fk.szxytkj.cn

TS:   arr.length
来源：http://sv.newstarts.cn

Java: list.size();
来源：http://ih.bookmarksfly.cn

Go:   len(arr)
来源：http://mp.hahajie.cn

Ruby: arr.length; arr.size
来源：http://dl.jctech888.com.cn

C#:   list.Count;
来源：http://tj.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://et.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://af.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xy.asd995.cn

JS:   arr.slice(1, 4);
来源：http://do.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ue.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://us.szsharing.cn

Go:   arr[1:4]
来源：http://xj.shxzukj.cn

Ruby: arr[1, 3]
来源：http://gk.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://zg.asd995.cn

[D08] 合并两个数组
来源：http://yn.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://ck.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://eh.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ts.haigaiapp.cn

TS:   [...a, ...b];
来源：http://qc.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gx.szxytkj.cn

Go:   append(a, b...)
来源：http://fg.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ex.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://is.shxzukj.cn

[D09] 排序（升序）
来源：http://uj.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://fb.colortex.cn

PHP:  sort($arr);
来源：http://dp.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cy.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ps.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lz.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gf.muxihuayi.cn

Ruby: arr.sort
来源：http://ju.jianghongdianzi.cn

C#:   list.Sort();
来源：http://bc.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hh.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://df.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://is.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yt.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dl.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rx.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ax.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jw.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sk.panjiajie.cn

[D11] 反转数组
来源：http://pg.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yd.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://jt.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pm.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://aj.lnxyls.cn

Java: Collections.reverse(list);
来源：http://rb.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://cp.wgjwhj.cn

Ruby: arr.reverse
来源：http://fw.shtwfgs.cn

C#:   list.Reverse();
来源：http://aw.521024.cn

[D12] 查找元素下标
来源：http://jb.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://bv.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xo.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ja.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gy.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tk.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ie.hahajie.cn

Ruby: arr.index(x)
来源：http://wz.521024.cn

C#:   list.IndexOf(x);
来源：http://op.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://bu.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://od.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://go.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://ow.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://pk.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gy.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rq.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tz.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wf.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://pr.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sm.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aa.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://mr.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://nv.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ls.nszjky.cn

Go:   // 手写循环
来源：http://ra.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dr.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://up.nszjky.cn

[D15] 去重
来源：http://fy.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://st.colortex.cn

PHP:  array_unique($arr);
来源：http://ni.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://nj.huanxung.cn

TS:   [...new Set(arr)]
来源：http://zc.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nk.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hj.bjjhwx.cn

Ruby: arr.uniq
来源：http://jn.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://sp.521024.cn

[D16] 求和与平均值
来源：http://za.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uy.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pl.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ri.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jq.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qx.colortex.cn

Go:   // 手写循环累加
来源：http://kh.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lq.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://qt.newstarts.cn

[D17] 最大值与最小值
来源：http://xv.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://qi.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://gx.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jp.shxzskj.cn

TS:   Math.max(...arr);
来源：http://kb.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bt.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wq.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://vr.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://os.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://nz.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lb.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://if.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yg.shxzskj.cn

TS:   nested.flat();
来源：http://ia.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wm.huixiangedu.cn

Go:   // 手写双层循环
来源：http://er.huixiangedu.cn

Ruby: nested.flatten
来源：http://wl.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ac.jctech888.com.cn

[D19] 按字段分组
来源：http://dt.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rx.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://as.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pa.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mk.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jz.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://sb.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jb.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ij.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://vu.gzmigu.cn

Py:   Counter(arr)
来源：http://wt.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://qd.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wj.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gv.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://us.newstarts.cn

Go:   // 手写 map[T]int
来源：http://ko.nszjky.cn

Ruby: arr.tally
来源：http://vn.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ar.newstarts.cn

[D21] 判断是否包含某元素
来源：http://jx.bjjhwx.cn

Py:   x in arr
来源：http://fk.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://sx.521024.cn

JS:   arr.includes(x)
来源：http://mu.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://no.nszjky.cn

Java: list.contains(x)
来源：http://jw.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://gy.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://cn.newstarts.cn

C#:   list.Contains(x)
来源：http://fc.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://bs.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ma.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cb.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bw.9csxet.cn

TS:   [...arr];
来源：http://ea.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://ly.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://su.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://ei.521024.cn

C#:   new List<int>(list);
来源：http://lx.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://bz.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://go.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xb.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fy.muxihuayi.cn


<!-- 参考信息 -->