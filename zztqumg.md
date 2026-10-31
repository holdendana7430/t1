代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://py.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rp.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jo.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://ll.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xp.asd995.cn

[C07] 把函数作为参数传入
来源：http://gn.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gf.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xr.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qu.nszjky.cn

TS:   arr.map(String)
来源：http://xe.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fv.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mj.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://fz.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fp.gzmigu.cn

[C08] 闭包
来源：http://ln.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cd.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ab.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iz.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pb.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cd.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xs.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ln.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://en.asd995.cn

[C09] 递归
来源：http://ft.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bb.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://za.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zn.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ho.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ng.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kh.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ks.yuntaijiaju.cn

[C10] 变量作用域
来源：http://wk.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://br.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tt.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ke.panjiajie.cn

TS:   同 JS
来源：http://tt.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://db.shxzskj.cn

Go:   花括号块级作用域
来源：http://fp.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xw.nszjky.cn

C#:   块级作用域
来源：http://oj.lnxyls.cn

[C11] 模块导入与导出
来源：http://jw.nicolike.cn

Py:   from module import func
来源：http://nj.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ff.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ab.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ak.521024.cn

Java: import java.util.List;
来源：http://va.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gk.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://kh.shxzukj.cn

C#:   using System.Text;
来源：http://ll.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://zo.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://bs.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://nh.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ji.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://uf.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ml.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://sh.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://oq.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yp.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://xr.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ws.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fm.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ww.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ei.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ae.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://uj.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yc.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jb.bookmarksfly.cn

[C14] 泛型函数
来源：http://bs.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ja.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://ao.bjjhwx.cn

JS:   // 无泛型
来源：http://mk.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ie.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hv.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qc.nszjky.cn

Ruby: # 无泛型
来源：http://vk.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ng.colortex.cn

[C15] 解构 / 展开参数
来源：http://ka.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cg.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://mi.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gm.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ce.nszjky.cn

Java: // 无解构
来源：http://zm.jianghongdianzi.cn

Go:   // 无解构
来源：http://rq.gzmigu.cn

Ruby: a, b = pair
来源：http://xg.newstarts.cn

C#:   var (a, b) = pair;
来源：http://gl.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://ao.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mh.asd995.cn

PHP:  // 无重载
来源：http://io.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uh.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://xj.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vy.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://mf.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://tt.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yx.yuexingan06.cn

================================================================================
来源：http://oy.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://tn.muxihuayi.cn

================================================================================
来源：http://cp.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://rj.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pt.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bf.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gi.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jt.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tg.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jt.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://by.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yt.shxzukj.cn

[D02] 追加元素到末尾
来源：http://jl.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cy.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xz.newstarts.cn

JS:   arr.push(4);
来源：http://od.hahajie.cn

TS:   arr.push(4);
来源：http://mk.nszjky.cn

Java: list.add(4);
来源：http://fw.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://lk.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://yo.haigaiapp.cn

C#:   list.Add(4);
来源：http://lv.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://nl.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://fl.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qv.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zg.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://uu.bjjhwx.cn

Java: list.add(0, 0);
来源：http://ub.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ye.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sd.521024.cn

C#:   list.Insert(0, 0);
来源：http://hi.hnjuh.cn

[D04] 删除元素
来源：http://sd.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zi.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hh.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hi.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://mw.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rp.bjjhwx.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ii.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wl.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vr.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://pn.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ug.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qs.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://en.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://zv.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://ew.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fv.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vr.hahajie.cn

[D06] 数组长度
来源：http://sv.hahajie.cn

Py:   len(arr)
来源：http://rs.lnxyls.cn

PHP:  count($arr);
来源：http://gv.haigaiapp.cn

JS:   arr.length
来源：http://ps.szsharing.cn

TS:   arr.length
来源：http://bk.huixiangedu.cn

Java: list.size();
来源：http://ty.yuexingan06.cn

Go:   len(arr)
来源：http://vf.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://pw.521024.cn

C#:   list.Count;
来源：http://sc.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ni.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sr.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qn.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://gt.colortex.cn

TS:   arr.slice(1, 4);
来源：http://kp.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://pc.muxihuayi.cn

Go:   arr[1:4]
来源：http://hi.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://ns.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://dy.shxzukj.cn

[D08] 合并两个数组
来源：http://bu.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://wf.asd995.cn

PHP:  array_merge($a, $b);
来源：http://pv.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tx.chemitech.net.cn

TS:   [...a, ...b];
来源：http://xh.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kn.shtwfgs.cn

Go:   append(a, b...)
来源：http://ct.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://ak.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://ai.bjjhwx.cn

[D09] 排序（升序）
来源：http://os.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://nw.gzmigu.cn

PHP:  sort($arr);
来源：http://vp.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ad.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://be.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pa.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dp.haigaiapp.cn

Ruby: arr.sort
来源：http://hw.huixiangedu.cn

C#:   list.Sort();
来源：http://dg.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://br.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rl.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yg.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://es.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tr.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zc.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bf.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tm.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sy.szxytkj.cn

[D11] 反转数组
来源：http://sy.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vo.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://yj.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ad.hahajie.cn

TS:   [...arr].reverse();
来源：http://sd.shxzskj.cn

Java: Collections.reverse(list);
来源：http://zp.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://mi.gzmigu.cn

Ruby: arr.reverse
来源：http://nb.hahajie.cn

C#:   list.Reverse();
来源：http://nm.huanxung.cn

[D12] 查找元素下标
来源：http://yf.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://sl.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dn.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xh.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ql.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iu.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://pd.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ia.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://wc.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://xg.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lv.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xe.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://ic.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://sv.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oj.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ou.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://du.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kd.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://ii.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fb.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xy.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ya.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://hv.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lq.lnxyls.cn

Go:   // 手写循环
来源：http://cg.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dl.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nl.huixinmuqiang.cn

[D15] 去重
来源：http://zy.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ib.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://cj.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://cc.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://pr.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kf.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yn.hnjuh.cn

Ruby: arr.uniq
来源：http://ks.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://dj.huanxung.cn

[D16] 求和与平均值
来源：http://ft.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vy.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yg.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pm.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ip.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xm.haigaiapp.cn

Go:   // 手写循环累加
来源：http://nh.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jh.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://qi.newstarts.cn

[D17] 最大值与最小值
来源：http://qv.521024.cn

Py:   max(arr);  min(arr)
来源：http://zk.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://np.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ai.shxzskj.cn

TS:   Math.max(...arr);
来源：http://zc.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qf.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bd.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://xz.asd995.cn

C#:   list.Max();  list.Min()
来源：http://vg.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://pf.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cp.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://zp.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xt.shxzukj.cn

TS:   nested.flat();
来源：http://hc.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vq.lnxyls.cn

Go:   // 手写双层循环
来源：http://ec.huixiangedu.cn

Ruby: nested.flatten
来源：http://av.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pg.panjiajie.cn

[D19] 按字段分组
来源：http://je.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bc.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nw.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xo.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://na.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://br.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://xk.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ew.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pt.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://th.szsharing.cn

Py:   Counter(arr)
来源：http://ad.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://tt.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://el.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vt.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jj.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://sh.huanxung.cn

Ruby: arr.tally
来源：http://ow.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xn.colortex.cn

[D21] 判断是否包含某元素
来源：http://wm.chemitech.net.cn

Py:   x in arr
来源：http://iv.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://yl.chemitech.net.cn

JS:   arr.includes(x)
来源：http://pl.huanxung.cn

TS:   arr.includes(x)
来源：http://fq.hnjuh.cn

Java: list.contains(x)
来源：http://al.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://pw.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://lm.gzmigu.cn

C#:   list.Contains(x)
来源：http://ht.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://xh.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ya.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://he.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://za.nszjky.cn

TS:   [...arr];
来源：http://xz.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://es.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lu.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://qx.wgjwhj.cn

C#:   new List<int>(list);
来源：http://yk.chemitech.net.cn

[D23] reduce 累积计算
来源：http://rl.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sb.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bo.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://og.jianghongdianzi.cn


<!-- 参考信息 -->