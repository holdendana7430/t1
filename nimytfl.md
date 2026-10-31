代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://lh.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://de.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ow.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://rh.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://as.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://hi.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ry.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bv.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qq.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://xr.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cn.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fb.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://xz.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rd.521024.cn

[C08] 闭包
来源：http://kc.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ad.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jo.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ik.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://im.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xe.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fh.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pk.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yg.lnxyls.cn

[C09] 递归
来源：http://zq.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tf.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://si.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uc.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mq.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hu.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://in.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mz.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://df.gzmigu.cn

[C10] 变量作用域
来源：http://bg.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://if.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mg.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hw.panjiajie.cn

TS:   同 JS
来源：http://vp.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://ib.wgjwhj.cn

Go:   花括号块级作用域
来源：http://uy.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fx.wgjwhj.cn

C#:   块级作用域
来源：http://il.nszjky.cn

[C11] 模块导入与导出
来源：http://mk.hahajie.cn

Py:   from module import func
来源：http://xm.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ls.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tc.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vz.hahajie.cn

Java: import java.util.List;
来源：http://eq.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ok.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://kr.huanxung.cn

C#:   using System.Text;
来源：http://cj.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://wq.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://fk.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://hb.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://oh.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://zh.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ny.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://ob.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://sr.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ex.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://pv.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vt.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vp.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nj.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gl.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ma.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yq.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nm.colortex.cn

[C14] 泛型函数
来源：http://oi.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ds.bjjhwx.cn

PHP:  // 无泛型
来源：http://ey.panjiajie.cn

JS:   // 无泛型
来源：http://ny.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gq.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nc.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uf.wgjwhj.cn

Ruby: # 无泛型
来源：http://it.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://co.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://bl.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ik.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://go.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ga.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://di.shtwfgs.cn

Java: // 无解构
来源：http://jp.9csxet.cn

Go:   // 无解构
来源：http://od.panjiajie.cn

Ruby: a, b = pair
来源：http://fg.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://tb.9csxet.cn

[C16] 函数 / 方法重载
来源：http://on.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dt.jctech888.com.cn

PHP:  // 无重载
来源：http://vq.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://av.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://ps.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nc.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://vf.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://hu.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oj.szxytkj.cn

================================================================================
来源：http://xm.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://yn.hahajie.cn

================================================================================
来源：http://td.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://ym.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ed.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ef.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uc.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vz.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qq.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jp.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://tc.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://iz.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cn.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tk.shxzukj.cn

JS:   arr.push(4);
来源：http://ir.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://bb.shxzskj.cn

Java: list.add(4);
来源：http://ja.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://ir.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://eo.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://cy.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://ek.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://qg.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://is.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jj.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://vt.bjjhwx.cn

Java: list.add(0, 0);
来源：http://tr.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ar.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bg.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://sw.huixinmuqiang.cn

[D04] 删除元素
来源：http://uh.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ps.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pi.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kp.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://jf.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pp.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://li.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vs.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gy.asd995.cn

[D05] 访问与修改元素
来源：http://ix.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sj.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ye.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zt.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ml.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://ab.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://ks.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xp.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://di.nszjky.cn

[D06] 数组长度
来源：http://my.shxzskj.cn

Py:   len(arr)
来源：http://vp.bookmarksfly.cn

PHP:  count($arr);
来源：http://rb.jctech888.com.cn

JS:   arr.length
来源：http://tb.yuntaijiaju.cn

TS:   arr.length
来源：http://ir.yuntaijiaju.cn

Java: list.size();
来源：http://fo.muxihuayi.cn

Go:   len(arr)
来源：http://ss.huanxung.cn

Ruby: arr.length; arr.size
来源：http://up.haigaiapp.cn

C#:   list.Count;
来源：http://sq.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://pv.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xd.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yv.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://nj.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ad.szxytkj.cn

Java: list.subList(1, 4);
来源：http://wj.lnxyls.cn

Go:   arr[1:4]
来源：http://yp.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://hu.521024.cn

C#:   list.GetRange(1, 3);
来源：http://dz.jctech888.com.cn

[D08] 合并两个数组
来源：http://bo.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://za.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://qj.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ss.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ei.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://or.colortex.cn

Go:   append(a, b...)
来源：http://mo.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://ez.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://fg.shxzukj.cn

[D09] 排序（升序）
来源：http://cr.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://bb.gzmigu.cn

PHP:  sort($arr);
来源：http://cm.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://po.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rr.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nq.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mz.jianghongdianzi.cn

Ruby: arr.sort
来源：http://wq.muxihuayi.cn

C#:   list.Sort();
来源：http://re.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xh.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://el.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yq.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mn.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ez.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hc.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bq.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pw.szsharing.cn

[D11] 反转数组
来源：http://rw.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://es.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://vt.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bi.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://bm.gzmigu.cn

Java: Collections.reverse(list);
来源：http://te.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://db.shtwfgs.cn

Ruby: arr.reverse
来源：http://pb.panjiajie.cn

C#:   list.Reverse();
来源：http://xr.521024.cn

[D12] 查找元素下标
来源：http://wq.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://yr.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lo.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ua.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://en.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wi.521024.cn

Go:   slices.Index(arr, x)
来源：http://xv.hnjuh.cn

Ruby: arr.index(x)
来源：http://dx.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://pb.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://td.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yi.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ph.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://yp.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://en.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://da.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xf.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yt.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ir.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://hg.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ek.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zz.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://ym.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://kw.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oc.wgjwhj.cn

Go:   // 手写循环
来源：http://jn.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tt.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qk.chemitech.net.cn

[D15] 去重
来源：http://ru.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ft.newstarts.cn

PHP:  array_unique($arr);
来源：http://pj.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://mh.huanxung.cn

TS:   [...new Set(arr)]
来源：http://wl.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mz.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eg.shxzukj.cn

Ruby: arr.uniq
来源：http://ci.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ln.muxihuayi.cn

[D16] 求和与平均值
来源：http://vq.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ml.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kg.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fs.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ff.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iw.szxytkj.cn

Go:   // 手写循环累加
来源：http://uc.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ez.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://vd.521024.cn

[D17] 最大值与最小值
来源：http://gn.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://cy.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://ev.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iu.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://fv.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pl.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pl.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://gl.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://wq.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://az.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vq.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://sf.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cm.nicolike.cn

TS:   nested.flat();
来源：http://cd.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pu.lnxyls.cn

Go:   // 手写双层循环
来源：http://ke.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://ib.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ah.yuntaijiaju.cn

[D19] 按字段分组
来源：http://qy.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ip.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ue.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pr.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://km.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yw.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://nz.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fn.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yi.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://gw.521024.cn

Py:   Counter(arr)
来源：http://yh.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://io.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fz.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ct.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://co.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://kq.hnjuh.cn

Ruby: arr.tally
来源：http://om.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zi.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://cn.yuntaijiaju.cn

Py:   x in arr
来源：http://xw.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ez.haigaiapp.cn

JS:   arr.includes(x)
来源：http://sh.huanxung.cn

TS:   arr.includes(x)
来源：http://ie.colortex.cn

Java: list.contains(x)
来源：http://up.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://sg.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://jn.szsharing.cn

C#:   list.Contains(x)
来源：http://yb.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://un.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://se.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mp.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://is.521024.cn

TS:   [...arr];
来源：http://ch.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://fv.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ov.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://km.muxihuayi.cn

C#:   new List<int>(list);
来源：http://dt.asd995.cn

[D23] reduce 累积计算
来源：http://ig.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ts.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zp.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uk.huanxung.cn


<!-- 参考信息 -->