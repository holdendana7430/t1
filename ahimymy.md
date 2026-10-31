代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ty.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://qj.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yq.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hl.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://il.szsharing.cn

TS:   arr.map(String)
来源：http://yj.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ck.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zn.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://hm.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://er.haigaiapp.cn

[C08] 闭包
来源：http://vw.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ov.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rk.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cl.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dd.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bm.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hq.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gc.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rz.szxytkj.cn

[C09] 递归
来源：http://do.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vh.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pt.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vg.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oc.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rx.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://md.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iy.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mo.szsharing.cn

[C10] 变量作用域
来源：http://mx.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hr.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ht.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cj.szxytkj.cn

TS:   同 JS
来源：http://gx.nszjky.cn

Java: 方法内为块级作用域
来源：http://dk.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://sf.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jp.huanxung.cn

C#:   块级作用域
来源：http://zo.9csxet.cn

[C11] 模块导入与导出
来源：http://od.huanxung.cn

Py:   from module import func
来源：http://gp.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vz.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vf.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pt.colortex.cn

Java: import java.util.List;
来源：http://gb.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ze.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://oe.huanxung.cn

C#:   using System.Text;
来源：http://qw.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://su.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://ob.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://lm.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://rb.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://td.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jq.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zs.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://oi.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://se.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://cl.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://st.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lj.panjiajie.cn

Go:   func add(a, b int) int
来源：http://yq.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zb.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ju.huanxung.cn

[C14] 泛型函数
来源：http://xp.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sy.wgjwhj.cn

PHP:  // 无泛型
来源：http://lx.newstarts.cn

JS:   // 无泛型
来源：http://ji.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://au.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ek.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gl.haigaiapp.cn

Ruby: # 无泛型
来源：http://ul.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qk.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://qm.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ju.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://em.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ek.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://as.colortex.cn

Java: // 无解构
来源：http://iv.asd995.cn

Go:   // 无解构
来源：http://cj.huixiangedu.cn

Ruby: a, b = pair
来源：http://ah.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://om.szsharing.cn

[C16] 函数 / 方法重载
来源：http://lv.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ow.asd995.cn

PHP:  // 无重载
来源：http://bw.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fu.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://bg.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nu.521024.cn

Go:   // 无重载：用不同函数名
来源：http://hi.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://kk.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://no.haigaiapp.cn

================================================================================
来源：http://rp.asd995.cn

D. 数组 / 列表 / 集合
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://wu.newstarts.cn

[D01] 创建数组 / 列表
来源：http://su.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lx.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yl.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jg.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tr.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pe.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://rr.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://ia.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wc.gzmigu.cn

[D02] 追加元素到末尾
来源：http://gb.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nl.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zx.colortex.cn

JS:   arr.push(4);
来源：http://xs.haigaiapp.cn

TS:   arr.push(4);
来源：http://zf.hahajie.cn

Java: list.add(4);
来源：http://sw.521024.cn

Go:   arr = append(arr, 4)
来源：http://fw.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://ki.szsharing.cn

C#:   list.Add(4);
来源：http://dw.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://fs.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://zq.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wq.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ks.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://pt.haigaiapp.cn

Java: list.add(0, 0);
来源：http://xw.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qk.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wr.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://sj.chemitech.net.cn

[D04] 删除元素
来源：http://mj.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aa.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ac.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zm.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://sv.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rl.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cq.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rl.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://if.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://dm.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gb.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://va.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ks.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://np.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://oy.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sm.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wd.nszjky.cn

[D06] 数组长度
来源：http://as.huixinmuqiang.cn

Py:   len(arr)
来源：http://fa.gzmigu.cn

PHP:  count($arr);
来源：http://hc.haigaiapp.cn

JS:   arr.length
来源：http://rh.lnxyls.cn

TS:   arr.length
来源：http://ab.jctech888.com.cn

Java: list.size();
来源：http://nl.huixiangedu.cn

Go:   len(arr)
来源：http://yk.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://wz.jianghongdianzi.cn

C#:   list.Count;
来源：http://qz.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://zz.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oc.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pd.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ge.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://mc.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ky.nicolike.cn

Go:   arr[1:4]
来源：http://or.lnxyls.cn

Ruby: arr[1, 3]
来源：http://fu.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://al.newstarts.cn

[D08] 合并两个数组
来源：http://dd.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://pe.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://oq.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zb.shtwfgs.cn

TS:   [...a, ...b];
来源：http://cm.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sj.asd995.cn

Go:   append(a, b...)
来源：http://dl.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://tj.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://yl.521024.cn

[D09] 排序（升序）
来源：http://bs.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.szsharing.cn

PHP:  sort($arr);
来源：http://lw.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rt.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cj.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xe.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tg.bjjhwx.cn

Ruby: arr.sort
来源：http://in.9csxet.cn

C#:   list.Sort();
来源：http://rw.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tb.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ch.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jn.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hu.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sg.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sh.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rl.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pf.gzmigu.cn

[D11] 反转数组
来源：http://qc.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xa.asd995.cn

PHP:  array_reverse($arr);
来源：http://cq.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mf.szxytkj.cn

TS:   [...arr].reverse();
来源：http://kp.colortex.cn

Java: Collections.reverse(list);
来源：http://sb.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://hw.shtwfgs.cn

Ruby: arr.reverse
来源：http://zi.muxihuayi.cn

C#:   list.Reverse();
来源：http://zj.shxzukj.cn

[D12] 查找元素下标
来源：http://gg.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://gu.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yg.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uk.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mu.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lw.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://fb.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://bb.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://pp.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://xs.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ns.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ux.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://fk.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://bv.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zz.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ox.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nk.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jb.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://op.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ek.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qb.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://dj.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://ve.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pt.chemitech.net.cn

Go:   // 手写循环
来源：http://iy.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dd.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ax.gzmigu.cn

[D15] 去重
来源：http://ri.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vx.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://ox.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://ko.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://wo.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vj.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yo.shtwfgs.cn

Ruby: arr.uniq
来源：http://im.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://pj.gzmigu.cn

[D16] 求和与平均值
来源：http://vr.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uf.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ql.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://te.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zy.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vd.shxzukj.cn

Go:   // 手写循环累加
来源：http://qe.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sp.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://mb.haigaiapp.cn

[D17] 最大值与最小值
来源：http://lv.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://in.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://wd.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dl.colortex.cn

TS:   Math.max(...arr);
来源：http://an.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uh.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xe.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://lb.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://ze.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://oi.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vt.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://tz.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vm.hnjuh.cn

TS:   nested.flat();
来源：http://wp.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zv.wgjwhj.cn

Go:   // 手写双层循环
来源：http://rh.bjjhwx.cn

Ruby: nested.flatten
来源：http://ri.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yd.jctech888.com.cn

[D19] 按字段分组
来源：http://fr.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mt.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uh.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fh.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fb.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oa.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://lt.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lt.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eu.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ab.chemitech.net.cn

Py:   Counter(arr)
来源：http://xf.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://eu.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lc.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cj.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pc.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://tu.newstarts.cn

Ruby: arr.tally
来源：http://xp.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oc.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://jz.chemitech.net.cn

Py:   x in arr
来源：http://dv.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://hl.chemitech.net.cn

JS:   arr.includes(x)
来源：http://to.jctech888.com.cn

TS:   arr.includes(x)
来源：http://hc.muxihuayi.cn

Java: list.contains(x)
来源：http://xg.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://yr.newstarts.cn

Ruby: arr.include?(x)
来源：http://le.hnjuh.cn

C#:   list.Contains(x)
来源：http://gh.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://bq.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lq.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gl.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bz.hahajie.cn

TS:   [...arr];
来源：http://qf.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://ab.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zm.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://dx.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://xw.colortex.cn

[D23] reduce 累积计算
来源：http://rc.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://if.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oh.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eb.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bu.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vw.shxzskj.cn

Go:   // 手写循环
来源：http://vf.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lk.yuexingan06.cn


<!-- 参考信息 -->