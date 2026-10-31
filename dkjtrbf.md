代发 wailian999

[C06] 匿名函数 / lambda
来源：http://sq.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://cb.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aa.shxzukj.cn

JS:   const square = x => x * x;
来源：http://nc.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://zr.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://py.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hd.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://rq.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yd.9csxet.cn

[C07] 把函数作为参数传入
来源：http://ja.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hl.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ay.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ja.521024.cn

TS:   arr.map(String)
来源：http://an.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ij.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bs.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://qe.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rk.gzmigu.cn

[C08] 闭包
来源：http://xc.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zd.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sd.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pk.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lm.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://we.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pd.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qe.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fi.shtwfgs.cn

[C09] 递归
来源：http://bj.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ka.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://om.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hg.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jr.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ri.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ez.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qp.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fq.shxzskj.cn

[C10] 变量作用域
来源：http://ss.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wt.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dk.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pg.521024.cn

TS:   同 JS
来源：http://xn.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://ch.huanxung.cn

Go:   花括号块级作用域
来源：http://ix.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ea.nszjky.cn

C#:   块级作用域
来源：http://np.huanxung.cn

[C11] 模块导入与导出
来源：http://qf.shtwfgs.cn

Py:   from module import func
来源：http://qz.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bd.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lj.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iu.huixinmuqiang.cn

Java: import java.util.List;
来源：http://fu.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jq.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://qu.muxihuayi.cn

C#:   using System.Text;
来源：http://bo.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://qv.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://hw.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://hq.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://fg.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://ym.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cy.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://pd.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://tr.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ep.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://pz.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bv.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gt.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ys.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nz.shxzskj.cn

Go:   func add(a, b int) int
来源：http://aq.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rz.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eb.shxzskj.cn

[C14] 泛型函数
来源：http://tp.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oj.9csxet.cn

PHP:  // 无泛型
来源：http://sf.shxzskj.cn

JS:   // 无泛型
来源：http://fm.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jo.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gw.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://be.huanxung.cn

Ruby: # 无泛型
来源：http://zh.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hs.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://dj.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fl.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://pi.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vx.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yn.nszjky.cn

Java: // 无解构
来源：http://cm.jianghongdianzi.cn

Go:   // 无解构
来源：http://fv.colortex.cn

Ruby: a, b = pair
来源：http://ay.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://wb.huanxung.cn

[C16] 函数 / 方法重载
来源：http://un.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rs.panjiajie.cn

PHP:  // 无重载
来源：http://lr.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vw.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://pb.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qu.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ul.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://qn.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ub.panjiajie.cn

================================================================================
来源：http://pn.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://wv.huanxung.cn

================================================================================
来源：http://mn.szsharing.cn

[D01] 创建数组 / 列表
来源：http://tt.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mt.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jm.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yk.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wh.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bn.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://me.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://bq.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nr.newstarts.cn

[D02] 追加元素到末尾
来源：http://xp.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tz.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jk.hahajie.cn

JS:   arr.push(4);
来源：http://ol.hnjuh.cn

TS:   arr.push(4);
来源：http://zc.chemitech.net.cn

Java: list.add(4);
来源：http://af.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://oe.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://fb.521024.cn

C#:   list.Add(4);
来源：http://xv.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://en.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://ga.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wm.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xi.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vw.colortex.cn

Java: list.add(0, 0);
来源：http://li.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wl.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lz.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ss.szsharing.cn

[D04] 删除元素
来源：http://br.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://se.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bl.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://il.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://vg.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ll.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fi.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://on.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nq.yuexingan06.cn

[D05] 访问与修改元素
来源：http://pd.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yc.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ny.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yb.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://gz.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://pz.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://bu.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ih.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gz.huanxung.cn

[D06] 数组长度
来源：http://jv.muxihuayi.cn

Py:   len(arr)
来源：http://jn.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ys.colortex.cn

JS:   arr.length
来源：http://mv.colortex.cn

TS:   arr.length
来源：http://qg.nicolike.cn

Java: list.size();
来源：http://vk.shtwfgs.cn

Go:   len(arr)
来源：http://hn.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://ja.newstarts.cn

C#:   list.Count;
来源：http://hz.hahajie.cn

[D07] 切片 / 取子数组
来源：http://eo.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aw.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ld.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://sd.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://fo.lnxyls.cn

Java: list.subList(1, 4);
来源：http://ls.jctech888.com.cn

Go:   arr[1:4]
来源：http://bi.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://kl.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://nl.yuexingan06.cn

[D08] 合并两个数组
来源：http://rr.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://yv.asd995.cn

PHP:  array_merge($a, $b);
来源：http://za.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yq.szsharing.cn

TS:   [...a, ...b];
来源：http://bd.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://et.bjjhwx.cn

Go:   append(a, b...)
来源：http://ze.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://gq.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://cu.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://nm.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ii.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://ul.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ab.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oj.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xu.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ow.asd995.cn

Ruby: arr.sort
来源：http://sz.panjiajie.cn

C#:   list.Sort();
来源：http://td.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ty.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xi.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://no.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qv.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pn.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sj.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yh.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bb.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ko.nicolike.cn

[D11] 反转数组
来源：http://rp.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://es.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://tz.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tp.nicolike.cn

TS:   [...arr].reverse();
来源：http://ns.nszjky.cn

Java: Collections.reverse(list);
来源：http://pi.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://zk.shxzskj.cn

Ruby: arr.reverse
来源：http://fi.hnjuh.cn

C#:   list.Reverse();
来源：http://jj.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://yx.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://ve.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kk.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dx.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://os.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://ox.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://vw.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://oq.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://md.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qv.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nt.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://nc.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://eg.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pp.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bc.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vo.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oh.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://xd.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lt.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ci.521024.cn

JS:   arr.map(x => x * 2)
来源：http://le.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://uf.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vq.asd995.cn

Go:   // 手写循环
来源：http://ew.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ge.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yw.huanxung.cn

[D15] 去重
来源：http://te.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oj.shxzskj.cn

PHP:  array_unique($arr);
来源：http://aw.huanxung.cn

JS:   [...new Set(arr)]
来源：http://eg.nszjky.cn

TS:   [...new Set(arr)]
来源：http://px.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nm.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sx.nicolike.cn

Ruby: arr.uniq
来源：http://nw.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://in.huixiangedu.cn

[D16] 求和与平均值
来源：http://ib.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xj.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zz.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vn.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lv.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zn.shtwfgs.cn

Go:   // 手写循环累加
来源：http://zu.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sj.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://nw.haigaiapp.cn

[D17] 最大值与最小值
来源：http://qt.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://eq.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://hd.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dx.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://ld.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fo.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xw.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ef.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://fq.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://uu.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zn.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://jz.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pv.hnjuh.cn

TS:   nested.flat();
来源：http://jt.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fw.szxytkj.cn

Go:   // 手写双层循环
来源：http://ja.colortex.cn

Ruby: nested.flatten
来源：http://ps.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jh.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ym.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vi.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tb.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nq.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ov.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mo.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://er.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://er.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vi.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://sv.shxzskj.cn

Py:   Counter(arr)
来源：http://hv.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ej.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sz.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cg.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xi.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://zc.chemitech.net.cn

Ruby: arr.tally
来源：http://xq.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mb.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://ra.jctech888.com.cn

Py:   x in arr
来源：http://rx.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://wc.panjiajie.cn

JS:   arr.includes(x)
来源：http://wc.colortex.cn

TS:   arr.includes(x)
来源：http://oi.panjiajie.cn

Java: list.contains(x)
来源：http://jy.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://zb.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://at.yuexingan06.cn

C#:   list.Contains(x)
来源：http://co.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://ar.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ym.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ak.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ci.newstarts.cn

TS:   [...arr];
来源：http://cm.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://gl.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jn.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://my.gzmigu.cn

C#:   new List<int>(list);
来源：http://dv.bjjhwx.cn


<!-- 参考信息 -->